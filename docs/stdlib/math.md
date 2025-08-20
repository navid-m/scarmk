# math

*Source: `math.scar`*

## Classes

### Vector2

A 2D vector.

#### Methods

##### init

`init(f32 x, f32 y)`

##### add

`add(ref math::Vector2 other) -> math`

Add two 2D vectors.

##### sub

`sub(ref math::Vector2 other) -> math`

Subtract two 2D vectors.

##### mul

`mul(ref math::Vector2 other) -> math`

Multiply two 2D vectors.

##### div

`div(ref math::Vector2 other) -> math`

Divide two 2D vectors.

### Vector3

A 3D vector.

#### Methods

##### init

`init(f32 x, f32 y, f32 z)`

##### add

`add(ref math::Vector3 other) -> math`

Add two 3D vectors.

##### sub

`sub(ref math::Vector3 other) -> math`

Subtract two 3D vectors.

##### mul

`mul(ref math::Vector3 other) -> math`

Multiply two 3D vectors.

##### div

`div(ref math::Vector3 other) -> math`

Divide two 3D vectors.

### Matrix3x2

### Matrix4x4


## Functions

### to_int

`to_int(string value) -> i32`

Convert string to 32-bit integer (supports optional +/-).

### to_float

`to_float(string value) -> f32`

Convert string to 32-bit float (supports optional +/- and decimals).

### min

`min(i32 a, i32 b) -> i32`

Minimum of two 32-bit integers.

### max

`max(i32 a, i32 b) -> i32`

Maximum of two 32-bit integers.

### absolute

`absolute(f32 value) -> f32`

Absolute value of a float.

### pow

`pow(f32 base, i32 exp) -> f32`

Power with integer exponent.

### factorial

`factorial(i32 n) -> i32`

Factorial of n; returns -1 for negative n.

### clamp

`clamp(f32 value, f32 min_value, f32 max_value) -> f32`

Clamp value to the inclusive range [min_value, max_value].

### normalize

`normalize(f32 x) -> f32`

Normalize angle in radians to (-PI, PI].

### sin

`sin(f32 x) -> f32`

Sine using a truncated Taylor series.

### cos

`cos(f32 x) -> f32`

Cosine using a truncated Taylor series.

### tan

`tan(f32 x) -> f32`

Will return 0.0 if cos(x) is too close to 0.0

### exp

`exp(f32 x) -> f32`

Exponential e^x using a series expansion.

### ln

`ln(f32 x) -> f32`

Natural logarithm; returns -1.0 for x <= 0.

### asin

`asin(f32 x) -> f32`

Arc sine; returns 0.0 if x is out of [-1, 1].

### acos

`acos(float x) -> float`

Arc cosine. Returns 0.0 if x is out of [-1, 1].

### atan

`atan(float x) -> float`

Arc tangent.

### atan2

`atan2(float y, float x) -> float`

Arc tangent of y/x using the signs of both to determine the quadrant.

### sqrt

`sqrt(f64 x) -> f64`

Square root using Newton's method
Will return -1.0 if x < 0.0

### round

`round(float value, int decimalPlaces) -> float`

Round to given decimal places (half up).

### print_float

`print_float(float value, int decimalPlaces) -> void`

Print float with specified number of decimal places without trailing zeroes
e.g. run math::print_float(3.14159265359, 2)

### mod

`mod(float a, float b) -> float`

Floating-point remainder a mod b.

### floor

`floor(float x) -> float`

Largest integer <= x.

### ceil

`ceil(float x) -> float`

Smallest integer >= x.

### log_base

`log_base(float x, float base) -> float`

Logarithm with arbitrary positive base; returns -1.0 on invalid input.

### radians

`radians(float degrees) -> float`

Convert degrees to radians.

### degrees

`degrees(float radians) -> float`

Convert radians to degrees.

### log10

`log10(float x) -> float`

Base-10 logarithm; returns -1.0 for x <= 0.

### log2

`log2(float x) -> float`

Base-2 logarithm; returns -1.0 for x <= 0.

### powf

`powf(float base, float exponent) -> float`

Power with float exponent using exp(exp * ln(base))
Returns 0.0 for non-positive base

### sqrtf

`sqrtf(float x) -> float`

Square root for float using Newton's method
Returns -1.0 if x < 0.0

### trunc

`trunc(float x) -> float`

### fract

`fract(float x) -> float`

Fractional part of x (x - floor(x)).

### sign

`sign(float x) -> int`

Sign of x: 1 for >0, -1 for <0, 0 otherwise.

### minf

`minf(float a, float b) -> float`

Minimum of two floats.

### maxf

`maxf(float a, float b) -> float`

Maximum of two floats.

### clampf

`clampf(float value, float min_value, float max_value) -> float`

Clamp float to the inclusive range [min_value, max_value].

### lerp

`lerp(float a, float b, float t) -> float`

Linear interpolation between a and b by t in [0,1].

### hypot

`hypot(float x, float y) -> float`

Hypotenuse sqrt(x*x + y*y).

### cbrt

`cbrt(float x) -> float`

Cube root using Newton's method.

### exp2

`exp2(float x) -> float`

2^x computed via e^(x*ln 2).

### sinh

`sinh(float x) -> float`

Hyperbolic sine.

### cosh

`cosh(float x) -> float`

Hyperbolic cosine.

### tanh

`tanh(float x) -> float`

Hyperbolic tangent.

