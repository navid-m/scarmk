# csv

*Source: `./csv.scar`*

## Imports

- `std/strings`
- `std/collections`
- `std/io`

## Classes

### CSVRow

#### Methods

##### add_field

`add_field(string field) -> void`

Add a field to the row.

##### get_field

`get_field(i32 index) -> string`

Get a field by index.

##### get_field_count

`get_field_count() -> i32`

Get the number of fields in the row.

##### set_field

`set_field(i32 index, string value) -> void`

Set a field at a specific index.

### CSV

#### Methods

##### add_row

`add_row(ref csv::CSVRow row) -> void`

Add a row to the CSV.

##### get_row

`get_row(i32 index) -> ref csv::CSVRow`

Get a row by index.

##### get_row_count

`get_row_count() -> i32`

Get the number of rows.

##### get_cell

`get_cell(i32 row, i32 col) -> string`

Get a specific cell value.

##### set_cell

`set_cell(i32 row, i32 col, string value) -> void`

Set a specific cell value.

##### resize

`resize() -> void`

Resize the internal row storage.


## Functions

### parse

`parse(string content) -> ref csv::CSV`

Parse CSV content into a CSV document using a comma delimiter.

### parse_with

`parse_with(string content, string delimiter) -> ref csv::CSV`

Parse CSV content with a custom single-character delimiter (use first char if longer).

### to_string

`to_string(ref csv::CSV doc) -> string`

Convert a CSV document to string using comma delimiter and CRLF newlines.

### to_string_with

`to_string_with(ref csv::CSV doc, string delimiter) -> string`

Convert a CSV document to string using a custom delimiter.

### read_file

`read_file(string filename) -> ref csv::CSV`

Read a CSV file (text) and parse it with comma delimiter.

### read_file_with

`read_file_with(string filename, string delimiter) -> ref csv::CSV`

Read a CSV file with a custom delimiter.

### write_file

`write_file(string filename, ref csv::CSV doc) -> bool`

Write a CSV document to a file using comma delimiter.

### write_file_with

`write_file_with(string filename, ref csv::CSV doc, string delimiter) -> bool`

Write a CSV document to a file with a custom delimiter.

