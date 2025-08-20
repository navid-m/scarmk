# collections

*Source: `collections.scar`*

## Classes

### class_name

#### Methods

##### init

`init(i32 initial_capacity)`

##### add_element

`add_element(elem_type value) -> void`

Add an element to the array.

##### get_element

`get_element(i32 index) -> elem_type`

Get an element from the array.

##### set_element

`set_element(i32 index, elem_type value) -> void`

Set an element in the array.

##### get_size

`get_size() -> i32`

Get the size of the array.

##### resize

`resize() -> void`

Resize the array.


## Macros

### NewArray

`NewArray(class_name, field_type, elem_type, cType, d_return, alloc_expr, free_expr, copy_expr, get_check)`

Define a new array type.


