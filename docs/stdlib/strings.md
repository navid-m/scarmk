# strings

*Source: `./strings.scar`*

## Imports

- `std/runtime`

## Classes

### Builder

#### Methods

##### append

`append(string str) -> void`

Appends a string to the builder.


## Macros

### get_char_at_either

`get_char_at_either(name, return_type)`

Returns the character at a specific index in a string.


## Functions

### length

`length(string str) -> int`

Returns the length of a string.

### compare

`compare(string a, string b) -> int`

Compares two strings.

### new_string_w_size

`new_string_w_size(string s, i32 size) -> string`

Quickly constructs a new string by copying the input.

If specific size is not needed, copy string using the fmt! builtin instead.

### ord

`ord(string str) -> int`

Returns the ordinal value of the first character of a string.

### ord_char

`ord_char(char c) -> int`

Returns the ordinal value of a character.

### chr

`chr(int ascii_value) -> char*`

Returns the character with the given ordinal value.

### trim_space

`trim_space(string str) -> lstring`

Trims leading and trailing whitespace from a string.

### trim_prefix

`trim_prefix(string str, string prefix) -> string`

Trims a prefix from a string.

### trim_suffix

`trim_suffix(lstring str, lstring suffix) -> lstring`

Trims a suffix from a string.

### ends_with

`ends_with(string str, string suffix) -> bool`

Checks if a string ends with a suffix.

### contains

`contains(string str, string substring) -> bool`

Checks if a string contains a substring.

### index_of

`index_of(lstring str, lstring substring) -> int`

Returns the index of the first occurrence of a substring in a string.

### last_index_of

`last_index_of(lstring str, lstring substring) -> int`

Returns the index of the last occurrence of a substring in a string.

### starts_with

`starts_with(string str, string prefix) -> bool`

Checks if a string starts with a prefix.

### substring

`substring(string str, int start, int end) -> char*`

Returns a substring of a string.

### to_hex

`to_hex(int value) -> char*`

Converts an integer to a hexadecimal string.

### from_hex

`from_hex(string hx) -> int`

Converts a hexadecimal string (like "2F" or "20") to an integer.

### equal

`equal(string a, string b) -> bool`

Compares two strings.

### replace

`replace(string str, string old_substr, string new_substr) -> char*`

Replaces all occurrences of a substring in a string.

### split

`split(string str, string delimiter) -> collections::StringArrayList`

Splits a string into a list of substrings.

### trim

`trim(string str) -> string`

Trims leading and trailing whitespace from a string.

### name

`name(string str, int index) -> return_type`

