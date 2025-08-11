# Parallel whiles

Parallel whiles can also be used to execute loop iterations concurrently as long as the loop condition holds, enabling efficient processing of tasks that may not have a predetermined iteration count.

```
pub i32 counter = 0
pub i32 limit = 400

parallel while counter < limit:
    print "Parallel counter: %d" | counter
    counter = counter + 1

print "Final counter: %d" | counter
```
