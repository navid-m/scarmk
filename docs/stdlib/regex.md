# regex

*Source: `regex.scar`*

## Imports

- `std/strings`
- `std/collections`

## Functions

### matches

`matches(string pattern, string text) -> bool`

Check if a string matches a regular expression pattern.

### find_joined

`find_joined(string pattern, string text) -> lstring`

Internal helper: returns all matches (full match and groups) joined by newlines.

### find

`find(string pattern, string text) -> collections`

Find all matches of a regular expression pattern in a string.

### replace

`replace(string pattern, string text, string replacement) -> char*`

Replace all matches of a regular expression pattern in a string.

Returns the modified string.

### split_joined

`split_joined(string pattern, string text) -> lstring`

Internal helper: split text by regex matches, returning pieces joined by newlines.

### split

`split(string pattern, string text) -> collections`

Split a string into a list of substrings using a regular expression pattern.

