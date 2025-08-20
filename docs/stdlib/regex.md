# regex

*Source: `regex.scar`*

## Functions

### matches

`matches(string pattern, string text) -> bool`

Check if a string matches a regular expression pattern.

### find

`find(string pattern, string text) -> list[string]`

Find all matches of a regular expression pattern in a string.

### replace

`replace(string pattern, string text, string replacement) -> char*`

Replace all matches of a regular expression pattern in a string.

Returns the modified string.

### split

`split(string pattern, string text) -> list[string]`

Split a string into a list of substrings using a regular expression pattern.

