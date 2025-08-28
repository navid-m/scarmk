# collections

*Source: `./collections.scar`*

## Imports

- `std/runtime`
- `std/math`

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

##### init

`init(i32 initial_capacity)`

##### find_index

`find_index(string key) -> i32`

Find the index of a key.

##### put

`put(string key, value_type value) -> void`

Add a key-value pair to the map.

##### get

`get(string key) -> value_type`

Get the value for a key.

##### contains_key

`contains_key(string key) -> bool`

Check if a key exists in the map.

##### remove

`remove(string key) -> void`

Remove a key-value pair from the map.

##### get_size

`get_size() -> i32`

Get the size of the map.

##### resize

`resize() -> void`

Resize the map.

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

##### init

`init(i32 initial_capacity)`

##### find_index

`find_index(string key) -> i32`

Find the index of a key.

##### put

`put(string key, value_type value) -> void`

Add a key-value pair to the map.

##### get

`get(string key) -> value_type`

Get the value for a key.

##### contains_key

`contains_key(string key) -> bool`

Check if a key exists in the map.

##### remove

`remove(string key) -> void`

Remove a key-value pair from the map.

##### get_size

`get_size() -> i32`

Get the size of the map.

##### resize

`resize() -> void`

Resize the map.


## Macros

### new_array

`new_array(class_name, field_type, elem_type, cType, d_return, alloc_expr, free_expr, copy_expr, get_check)`

Define a new array type.

### define_arraylist

`define_arraylist(class_name, elem_type, default_value)`

Convenience macro to define an ArrayList for a custom type.

Usage: define_arraylist(MyList, MyType, default_value)

Notes:

 - For most value types (including user-defined structs/classes that map to a C type),
   this will Just Work (TM) by using sizeof(elem_type) and plain assignment.

 - For strings, prefer the existing `StringArrayList` specialization.

### define_map

`define_map(class_name, value_type, cValueType, default_value)`

Convenience macro to define a string-keyed map for a custom value type.

Usage: define_map(MyMap, MyValueType, MyCType, default_value)

Notes:

 - Keys are strings and are strdup/free managed.

 - Values are stored by value; no destructor/free is invoked for values.

### define_vararg_array_init

`define_vararg_array_init(func_name, list_class, elem_type, convert_expr)`

Macro to define typed varargs array initializers.

Usage example:

define_vararg_array_init(init_array_i32, collections::ArrayList, i32, math::to_int(s))


## Functions

### func_name

`func_name(i32 count, ...) -> list_class`

