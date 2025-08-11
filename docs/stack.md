# Stack Allocation

### Overall Syntax

```
stallocate <data-type> <variable-name> = <size-as-number>
```

Stack allocation can be carried out using the `stallocate` keyword, where `<data-type>` can also be `ref <data-type>`.

### Example

An example of this is below:

```
fn process_block(int initial_permutation_index, int block_size) -> void:
    stallocate int local_count = this.n
    stallocate i8 local_temp_permutation = this.n
    stallocate i8 local_current_permutation = this.n

    int local_max_flip_count = 0
    int local_checksum = 0

    local_count[0] = 0
    for i = 0 to (this.n - 1):
        local_current_permutation[i] = i
```
