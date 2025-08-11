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
