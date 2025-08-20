# json

*Source: `json.scar`*

## Functions

### parse

`parse(string json_string) -> void*`

Parse JSON string and return json_t pointer

### loadup_file

`loadup_file(string filename) -> void*`

Parse JSON from file and return json_t pointer

### to_string

`to_string(void* json_obj) -> string`

Convert json_t to string representation

### to_string_pretty

`to_string_pretty(void* json_obj) -> string`

Convert json_t to pretty-printed string

### save_to_file

`save_to_file(void* json_obj, string filename) -> bool`

Save json_t to file

### get_type

`get_type(void* json_obj) -> i32`

Get the type of a JSON value

### check_is_object

`check_is_object(void* json_obj) -> bool`

Check if JSON value is of specific type

### check_is_array

`check_is_array(void* json_obj) -> bool`

### check_is_string

`check_is_string(void* json_obj) -> bool`

### check_is_integer

`check_is_integer(void* json_obj) -> bool`

### check_is_real

`check_is_real(void* json_obj) -> bool`

### check_is_number

`check_is_number(void* json_obj) -> bool`

### check_is_true

`check_is_true(void* json_obj) -> bool`

### check_is_false

`check_is_false(void* json_obj) -> bool`

### check_is_boolean

`check_is_boolean(void* json_obj) -> bool`

### check_is_null

`check_is_null(void* json_obj) -> bool`

### new_object

`new_object() -> void*`

Create JSON values

### new_array

`new_array() -> void*`

### new_string

`new_string(string value) -> void*`

### new_integer

`new_integer(i64 value) -> void*`

### new_real

`new_real(f64 value) -> void*`

### new_true

`new_true() -> void*`

### new_false

`new_false() -> void*`

### new_boolean

`new_boolean(bool value) -> void*`

### new_null

`new_null() -> void*`

### get_string_value

`get_string_value(void* json_obj) -> string`

Extract values from JSON

### get_integer_value

`get_integer_value(void* json_obj) -> i64`

### get_real_value

`get_real_value(void* json_obj) -> f64`

### get_number_value

`get_number_value(void* json_obj) -> f64`

### get_boolean_value

`get_boolean_value(void* json_obj) -> bool`

### obj_get

`obj_get(void* json_obj, string key) -> void*`

Object operations

### obj_set

`obj_set(void* json_obj, string key, void* value) -> bool`

### obj_set_new

`obj_set_new(void* json_obj, string key, void* value) -> bool`

### obj_del

`obj_del(void* json_obj, string key) -> bool`

### obj_clear

`obj_clear(void* json_obj) -> bool`

### obj_size

`obj_size(void* json_obj) -> i32`

### arr_get

`arr_get(void* json_array, i32 index) -> void*`

Array operations

### arr_set

`arr_set(void* json_array, i32 index, void* value) -> bool`

### arr_set_new

`arr_set_new(void* json_array, i32 index, void* value) -> bool`

### arr_append

`arr_append(void* json_array, void* value) -> bool`

### arr_append_new

`arr_append_new(void* json_array, void* value) -> bool`

### arr_insert

`arr_insert(void* json_array, i32 index, void* value) -> bool`

### arr_insert_new

`arr_insert_new(void* json_array, i32 index, void* value) -> bool`

### arr_remove

`arr_remove(void* json_array, i32 index) -> bool`

### arr_clear

`arr_clear(void* json_array) -> bool`

### arr_size

`arr_size(void* json_array) -> i32`

### inc_ref

`inc_ref(void* json_obj) -> void*`

Memory management

### dec_ref

`dec_ref(void* json_obj) -> void`

This will also delete objects created with dump_to_file

### get_object_string

`get_object_string(void* json_obj, string key) -> string`

Utility function for easier usage, get object string

### get_object_integer

`get_object_integer(void* json_obj, string key) -> i64`

Utility function for easier usage, get object integer

### get_object_real

`get_object_real(void* json_obj, string key) -> f64`

Utility function for easier usage, get object real

### get_object_boolean

`get_object_boolean(void* json_obj, string key) -> bool`

Utility function for easier usage, get object boolean

