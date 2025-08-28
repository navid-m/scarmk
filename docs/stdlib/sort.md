# sort

*Source: `./sort.scar`*

## Imports

- `std/math`
- `std/collections`

## Functions

### merge_int

`merge_int(ref i32 arr, i32 left, i32 mid, i32 right) -> void`

Merge function for merge sort

### sort_int_list

`sort_int_list(ref collections::ArrayList input_list) -> collections::ArrayList`

Sort a list of integers and return the sorted list
Uses bubble sort algorithm implemented in pure Scar

