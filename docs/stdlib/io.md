# io

*Source: `io.scar`*

## Imports

- `std/math`
- `std/collections`
- `std/strings`

## Functions

### readln

Read a line from stdin without the trailing newline.

### readln_with_prompt

Print a prompt then read a line from stdin.

### read_int

Read a line from stdin and parse it as 32-bit integer.

### read_float

Read a line from stdin and parse it as 32-bit float.

### read_bool

Read a line from stdin and parse it as boolean ("true" => true).

### read_char

Read a line and return its first character.

### read_split

Read a line and split it by the given delimiter.

### write_file

Write (overwrite) text content to a file. Returns true on success.

### append_file

Append text content to a file. Returns true on success.

### read_file

Read entire file content as a string.

### exists

Check if a file at the given path exists (readable).

