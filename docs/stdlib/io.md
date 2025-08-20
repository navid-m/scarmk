# io

*Source: `io.scar`*

## Imports

- `std/math`
- `std/collections`
- `std/strings`

## Functions

### readln

`readln() -> lstring`

Read a line from stdin without the trailing newline.

### readln_with_prompt

`readln_with_prompt(string prompt) -> lstring`

Print a prompt then read a line from stdin.

### read_int

`read_int() -> i32`

Read a line from stdin and parse it as 32-bit integer.

### read_float

`read_float() -> f32`

Read a line from stdin and parse it as 32-bit float.

### read_bool

`read_bool() -> bool`

Read a line from stdin and parse it as boolean ("true" => true).

### read_char

`read_char() -> char`

Read a line and return its first character.

### read_split

`read_split(char* delimiter) -> collections`

Read a line and split it by the given delimiter.

### write_file

`write_file(string filepath, string content) -> bool`

Write (overwrite) text content to a file. Returns true on success.

### append_file

`append_file(string filepath, string content) -> bool`

Append text content to a file. Returns true on success.

### read_file

`read_file(string filepath) -> lstring`

Read entire file content as a string.

### exists

`exists(string filepath) -> bool`

Check if a file at the given path exists (readable).

### to_stderr

`to_stderr(string message) -> void`

Send a string to the stderr stream

