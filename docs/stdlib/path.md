# path

*Source: `path.scar`*

## Classes

### PathParts

The base name and directory name of a path.


## Functions

### is_absolute_path

`is_absolute_path(string path) -> bool`

Check if a path is absolute.

### is_relative

`is_relative(string path) -> bool`

Check if a path is relative.

### extension

`extension(string path) -> char*`

Get the extension of a path.

### without_extension

`without_extension(string path) -> char*`

Get the path without extension.

### join

`join(string base, string relative) -> char*`

Join two paths.

### normalize

`normalize(string path) -> char*`

Normalize a path (remove //, ./, resolve ../ where possible).

### resolve

`resolve(string base, string rel) -> char*`

Resolve a relative path against a base path into an absolute.

### relative

`relative(string from, string to) -> char*`

Get the relative path from one path to another.

### basename

`basename(string path) -> char*`

Get the base name of a path.

### dirname

`dirname(string path) -> char*`

Get the directory name of a path.

### split

`split(string path) -> path`

Split a path into (dirname, basename).

