# Primitive Data Types

## i32

`i32` is a 32-bit signed integer type. It can represent whole numbers in the range from -2,147,483,648 to 2,147,483,647. This type is commonly used for numeric values where memory efficiency and performance are important, and negative values may be required.

## i16

`i16` is a 16-bit signed integer type. It can represent whole numbers in the range from -32,768 to 32,767. This type is useful when you need to save memory and the range of values fits within these limits.

## u32

`u32` is a 32-bit unsigned integer type. It can represent whole numbers from 0 to 4,294,967,295. Use this type when you need a large range of positive numbers and do not require negative values.

## u16

`u16` is a 16-bit unsigned integer type. It can represent whole numbers from 0 to 65,535. This type is suitable for small positive numbers and is often used for indexing or representing data where negative values are not needed.

## f32

`f32` is a 32-bit floating-point type. It can represent fractional numbers (numbers with decimals) with approximately 7 decimal digits of precision. Use `f32` when you need to store real numbers and memory usage is a concern.

## f64

`f64` is a 64-bit floating-point type. It can represent fractional numbers with approximately 15 decimal digits of precision. `f64` is the default floating-point type in many languages and is preferred when higher precision is required.

## string

`string` is essentially a pure C-style string in the style of `char*`
. It represents a sequence of characters terminated by a null byte (`\0`). Strings are used to store and manipulate text data. Since they are pointers to memory, care must be taken to manage memory allocation and deallocation to avoid leaks or buffer overflows. Operations such as concatenation, comparison, and length calculation are typically performed using standard library functions.

## bool

`bool` is a boolean type that can hold one of two values: `true` or `false`. It is commonly used for logical operations, conditional statements, and representing binary states.

## byte

`byte` is an 8-bit unsigned integer type, equivalent to `uint8_t` in C. It can represent values from 0 to 255 and is often used for raw data, buffers, or binary protocols.

## char

`char` is a single 8-bit character type, typically used to represent individual ASCII characters. It is the building block of strings and can also be used for character manipulation.

## Example Table

| Type   | Size (bits) | Signed | Range / Description                     |
| ------ | ----------- | ------ | --------------------------------------- |
| i32    | 32          | Yes    | -2,147,483,648 to 2,147,483,647         |
| i16    | 16          | Yes    | -32,768 to 32,767                       |
| u32    | 32          | No     | 0 to 4,294,967,295                      |
| u16    | 16          | No     | 0 to 65,535                             |
| f32    | 32          | N/A    | ~7 decimal digits precision             |
| f64    | 64          | N/A    | ~15 decimal digits precision            |
| string | N/A         | N/A    | Sequence of characters, null-terminated |
| bool   | 8           | N/A    | `true` or `false`                       |
| byte   | 8           | No     | 0 to 255                                |
| char   | 8           | N/A    | Single ASCII character                  |
