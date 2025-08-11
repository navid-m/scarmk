# Heap

### Overall Syntax

```
allocate <data-type> <variable-name> = <size-as-number>
```

Allocation can be carried out on the heap using the `allocate` keyword.

### Example

An example of this is below:

```
fn random_fasta(ref AminoAcid genelist, int genelist_len, int count) -> void:
    allocate f64 rb = RANDOM_BUF_SIZE
    allocate u8 wb = OUT_BUF_SIZE

    while count > 0:
        int chunk = min(count, RANDOM_BUF_SIZE)
        count = count - chunk
        generate_random(rb, chunk)
        int output_len = generate_dna(genelist, genelist_len, rb, wb, chunk)
        for i = 0 to (output_len - 1):
            print "%c" | wb[i]
```
