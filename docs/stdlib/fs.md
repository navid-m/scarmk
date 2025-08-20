# fs

*Source: `fs.scar`*

## Imports

- `std/strings`

## Functions

### make_dir

`make_dir(string path) -> bool`

Create a directory at the given path. Returns true on success.

### remove_dir

`remove_dir(string path) -> bool`

Remove an empty directory. Returns true on success.

### read_bytes

`read_bytes(string filename) -> list[int]`

Read entire file as bytes. Returns list of byte values (0-255).

### write_bytes

`write_bytes(string filename, list[int] data) -> bool`

Write bytes to a file. Overwrites existing file. Returns true on success.

### exists

`exists(string path) -> bool`

Check if a file or directory exists at path.

### remove

`remove(string path) -> bool`

Remove a file at the given path. Returns true on success.

### read_lines

`read_lines(string filename) -> list[string]`

Read a text file into a list of lines (without trailing newlines).

### list_dir

`list_dir(string path) -> list[string]`

List directory entries (files and subdirectories). Excludes . and ..

