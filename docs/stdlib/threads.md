# threads

*Source: `threads.scar`*

## Classes

### Thread

### Mutex


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

### mutex_unlock

### mutex_destroy

### sleep_ms

Sleep for the specified milliseconds

### yield_thread

Yield current thread's time slice

### num_cpus

Number of logical CPUs available

### current_thread_id

Get current thread id as 64-bit value

