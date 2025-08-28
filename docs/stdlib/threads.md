# threads

*Source: `./threads.scar`*

## Classes

### Thread

### Mutex


## Functions

### spawn

`spawn(i64 func_ptr, i64 arg_ptr) -> threads::Thread`

Spawn a native thread to run a C function pointer with an argument pointer.

WARNING: func_ptr must be a native function pointer compatible with the platform:

- Windows: DWORD WINAPI fn(void* arg)

- Unix:    void* fn(void* arg)


### join

`join(threads::Thread t)`

Join a thread created by spawn()

### detach

`detach(threads::Thread t)`

Detach a thread (cannot be joined afterward)

### mutex_create

`mutex_create() -> threads::Mutex`

Create a mutex

### mutex_lock

`mutex_lock(threads::Mutex m)`

Lock a mutex. Blocks until the lock is acquired.

### mutex_unlock

`mutex_unlock(threads::Mutex m)`

Unlock a mutex.

### mutex_destroy

`mutex_destroy(threads::Mutex m)`

Destroy a mutex and free its underlying resources.

### sleep_ms

`sleep_ms(i32 ms)`

Sleep for the specified milliseconds

### yield_thread

`yield_thread()`

Yield current thread's time slice

### num_cpus

`num_cpus() -> i32`

Number of logical CPUs available

### current_thread_id

`current_thread_id() -> u64`

Get current thread id as 64-bit value

