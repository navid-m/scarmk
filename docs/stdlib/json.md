# json

*Source: `lib/json.scar`*

## Functions

### parse

Parse JSON string and return json_t pointer

### loadup_file

Parse JSON from file and return json_t pointer

### to_string

Convert json_t to string representation

### to_string_pretty

Convert json_t to pretty-printed string

### save_to_file

Save json_t to file

### get_type

Get the type of a JSON value

### check_is_object

Check if JSON value is of specific type

### check_is_array

### check_is_string

### check_is_integer

### check_is_real

### check_is_number

### check_is_true

### check_is_false

### check_is_boolean

### check_is_null

### new_object

Create JSON values

### new_array

### new_string

### new_integer

### new_real

### new_true

### new_false

### new_boolean

### new_null

### get_string_value

Extract values from JSON

### get_integer_value

### get_real_value

### get_number_value

### get_boolean_value

### obj_get

Object operations

### obj_set

### obj_set_new

### obj_del

### obj_clear

### obj_size

### arr_get

Array operations

### arr_set

### arr_set_new

### arr_append

### arr_append_new

### arr_insert

### arr_insert_new

### arr_remove

### arr_clear

### arr_size

### inc_ref

Memory management

### dec_ref

This will also delete objects created with dump_to_file

### get_object_string

Utility functions for easier usage

### get_object_integer

### get_object_real

### get_object_boolean

