# threads

*Source: `threads.scar`*

## Classes

### Thread

Represents some thread.

### Mutex

Represents some mutex.


## Functions

### spawn

Spawn a native thread to run a C function pointer with an argument pointer.

WARNING: func_ptr must be a native function pointer compatible with the platform:

- Windows: DWORD WINAPI fn(void* arg)

- Unix:    void* fn(void* arg)


### join

Join a thread created by spawn()

### detach

Detach a thread (cannot be joined afterward)

### mutex_create

Create a mutex

### mutex_lock

Lock a mutex. Blocks until the lock is acquired.

### mutex_unlock

Unlock a mutex.

### mutex_destroy

Destroy a mutex and free its underlying resources.

### sleep_ms

Sleep for the specified milliseconds

### yield_thread

Yield current thread's time slice

### num_cpus

Number of logical CPUs available

### current_thread_id

Get current thread id as 64-bit value

