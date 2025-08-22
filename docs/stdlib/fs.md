# fs

*Source: `fs.scar`*

## Imports

- `std/strings`
- `std/io`
- `std/collections`

## Functions

### make_dir

`make_dir(string path) -> bool`

Create a directory at the given path. Returns true on success.

### remove_dir

`remove_dir(string path) -> bool`

Remove an empty directory. Returns true on success.

### read_bytes

`read_bytes(string filename) -> collections`

Read entire file as bytes. Returns ByteArrayList of u8 values.

### write_bytes

`write_bytes(string filename, collections::ArrayList data) -> bool`

Write bytes to a file. Overwrites existing file. Returns true on success.

### exists

`exists(string path) -> bool`

Check if a file or directory exists at path.

### remove

`remove(string path) -> bool`

Remove a file at the given path. Returns true on success.

### read_lines

`read_lines(string filename) -> collections`

Read a text file into a list of lines (without trailing newlines).

### list_dir_joined

`list_dir_joined(string path) -> lstring`

Internal helper: returns directory entries joined by newlines. Excludes . and ..

### list_dir

`list_dir(string path) -> collections`

List directory entries (files and subdirectories). Excludes . and ..

