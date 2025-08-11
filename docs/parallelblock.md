### Parallel block

The parallel block can be used alone in order to parallelize a set of executable statements.

```
parallel:
    print "Task 1 running"
    print "Task 2 running"
    for i = 0 to 5:
        print "Loop iteration: %d" | i

print "After parallel block"
```

This is highly useful in cases where you want to execute multiple independent tasks simultaneously, such as performing computations, handling I/O operations, or processing data in parallel to improve performance and reduce overall execution time. By leveraging the parallel block, you can maximize resource utilization and make your programs more efficient, especially on multi-core systems.
