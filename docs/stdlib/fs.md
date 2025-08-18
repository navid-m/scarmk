# fs

*Source: `fs.scar`*

## Imports

- `std/strings`

## Functions

### make_dir

Create a directory at the given path. Returns true on success.

### remove_dir

Remove an empty directory. Returns true on success.

### read_bytes

Read entire file as bytes. Returns list of byte values (0-255).

### write_bytes

Write bytes to a file. Overwrites existing file. Returns true on success.

### exists

Check if a file or directory exists at path.

### remove

Remove a file at the given path. Returns true on success.

### read_lines

Read a text file into a list of lines (without trailing newlines).

### list_dir

List directory entries (files and subdirectories). Excludes . and ..

