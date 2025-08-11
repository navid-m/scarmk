# Philosophy

### Why design another programming language?

Languages like Nim, Swift, and many others often leave concurrency and high-performance numeric computing to libraries or ad-hoc patterns. That forces users to stitch together: a language with ergonomic syntax + a heavy external lib (Arraymancer), and runtime/ABI mismatches.

The key point is this: A language that bakes in structured parallelism and numeric-first value semantics reduces that friction and enables far cleaner, higher-performance code by default.

Structured concurrency as primary model. parallel: and parallel for are essentially structured fork-join. This is simple to reason about, maps well to work-stealing runtimes, and composes easily with nested loops. It also allows the compiler to generate efficient join points.

### Justifications

#### Designing a language with concurrency and parallelism as a core construct

Compiler-first synchronization is a highly important design goal in Scar. Rather than forcing manual mutexes everywhere, the compiler performs static analysis (and when needed, emits runtime synchronization). But crucially you must combine static checks + opt-in/opt-out mechanisms:

-  Static detection of obvious races: if a variable is accessed from multiple concurrent tasks without synchronization, the compiler warns/error.
-  Automatic safe transforms: for a pattern like independent loop iterations updating a per-iteration slot, compiler can use thread-local buffers and a final merge to avoid locks.
-  Explicit annotations for intent: atomic, shared, reduction, or unique qualifiers let the compiler emit low-overhead atomics or lock-free code when you mean it.

#### Data-race-free and Sequential-consistency semantics

DRF / SC semantics are employed for usability. Adopting an easily-understood memory model. Sequential Consistency for Data-Race-Free (SC-for-DRF) by default (if program is data-race-free, it behaves like SC), while providing atomics and fences for low-level control. SC-for-DRF is easier for users and can be enforced via compile-time checks and sanitizer/runtime options.

Value-semantics, stack allocation, and escape analysis. To avoid "ref object everywhere" boxing:

-  Strong static typing with first-class value types (structs, arrays) that default to stack/inline allocation.
-  Escape analysis to determine when heap allocation is necessary.
-  Cheap move/borrow semantics (borrow or move, not implicit ref) to avoid copies while remaining safe.
-  Optional small-boxing for polymorphism/heterogeneous containers.

#### Compilation model

C backend for practical reasons.

Pros:

-  easy bootstrap
-  ubiquitous toolchain
-  interop with C libs (BLAS, pthreads)
-  simple debugging.

An LLVM backend will be adopted at a later stage of development.
