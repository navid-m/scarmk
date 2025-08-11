# Parallelism

### Parallel for

Parallel fors are useful for executing the same operation independently across multiple iterations, allowing computations to be performed concurrently and improving performance on multi-core systems.

```
parallel for i = 0 to 10:
    print "%d" | i
```

### Reduce clause

The reduce clause can be used to combine the results of parallel computations into a single value, such as summing partial results from each parallel task into a total.

```
parallel for t = 0 to (NO_TASKS - 1) reduce(sum: total_check):
    int check = 0
    for i32 j = n; j >= 1; j--:
        ref TreeNode tree = TreeNode::bottom_up_tree(depth)
        check = check + tree.item_check()
    total_check = total_check + check
```

### Parallel whiles

```
pub int counter = 0
pub int limit = 400

parallel while counter < limit:
    print "Parallel counter: %d" | counter
    counter = counter + 1

print "Final counter: %d" | counter
```
