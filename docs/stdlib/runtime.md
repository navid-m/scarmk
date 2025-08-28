# runtime

*Source: `./runtime.scar`*

## Functions

### error

`error(string msg)`

Print a runtime error message and exit with code 1.

### pointer_width

`pointer_width() -> int`

Get the native pointer width in bits (e.g., 32 or 64).

### is_little_endian

`is_little_endian() -> bool`

Determine if the machine is little-endian.

