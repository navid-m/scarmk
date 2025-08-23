# test

*Source: `test.scar`*

## Imports

- `std/math`
- `std/strings`

## Classes

### UnitTest

#### Methods

##### assert

`assert(bool condition, string message) -> void`

Assert that a condition is true.

##### assert_equals

`assert_equals(int expected, int actual, string message) -> void`

Assert that two integers are equal.

##### assert_string_equals

`assert_string_equals(string expected, string actual, string message) -> void`

Assert that two strings are equal.


## Functions

### assert_int_equals

`assert_int_equals(int expected, int actual, string message) -> void`

Assert that two integers are equal.

### assert_float_equals

`assert_float_equals(float expected, float actual, float tolerance, string message) -> void`

Assert that two floats are equal within a specified tolerance.

### assert_true

`assert_true(bool condition, string message) -> void`

Assert that a condition is true.

### assert_false

`assert_false(bool condition, string message) -> void`

Assert that a condition is false.

### assert_int_list_equals

`assert_int_list_equals(ref list[int] expected, ref list[int] actual, string message) -> void`

Assert that two integer lists are equal.

### test_summary

`test_summary() -> void`

Print a summary of the test results.

