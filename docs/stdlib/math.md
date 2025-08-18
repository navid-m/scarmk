# math

*Source: `math.scar`*

## Classes

### Vector2

A 2D vector.

#### Methods

##### init

##### add

Add two 2D vectors.

##### sub

Subtract two 2D vectors.

##### mul

Multiply two 2D vectors.

##### div

Divide two 2D vectors.

### Vector3

A 3D vector.

#### Methods

##### init

##### add

Add two 3D vectors.

##### sub

Subtract two 3D vectors.

##### mul

Multiply two 3D vectors.

##### div

Divide two 3D vectors.

### Matrix3x2

### Matrix4x4


## Functions

### to_int

Convert string to 32-bit integer (supports optional +/-).

### to_float

Convert string to 32-bit float (supports optional +/- and decimals).

### min

Minimum of two 32-bit integers.

### max

Maximum of two 32-bit integers.

### absolute

Absolute value of a float.

### pow

Power with integer exponent.

### factorial

Factorial of n; returns -1 for negative n.

### clamp

Clamp value to the inclusive range [min_value, max_value].

### normalize

Normalize angle in radians to (-PI, PI].

### sin

Sine using a truncated Taylor series.

### cos

Cosine using a truncated Taylor series.

### tan

Will return 0.0 if cos(x) is too close to 0.0

### exp

Exponential e^x using a series expansion.

### ln

Natural logarithm; returns -1.0 for x <= 0.

### asin

Arc sine; returns 0.0 if x is out of [-1, 1].

### acos

Arc cosine. Returns 0.0 if x is out of [-1, 1].

### atan

Arc tangent.

### atan2

Arc tangent of y/x using the signs of both to determine the quadrant.

### sqrt

Square root using Newton's method
Will return -1.0 if x < 0.0

### round

Round to given decimal places (half up).

### print_float

Print float with specified number of decimal places without trailing zeroes
e.g. run math::print_float(3.14159265359, 2)

### mod

Floating-point remainder a mod b.

### floor

Largest integer <= x.

### ceil

Smallest integer >= x.

### log_base

Logarithm with arbitrary positive base; returns -1.0 on invalid input.

### radians

Convert degrees to radians.

### degrees

Convert radians to degrees.

### log10

Base-10 logarithm; returns -1.0 for x <= 0.

### log2

Base-2 logarithm; returns -1.0 for x <= 0.

### powf

Power with float exponent using exp(exp * ln(base))
Returns 0.0 for non-positive base

### sqrtf

Square root for float using Newton's method
Returns -1.0 if x < 0.0

### trunc

### fract

Fractional part of x (x - floor(x)).

### sign

Sign of x: 1 for >0, -1 for <0, 0 otherwise.

### minf

Minimum of two floats.

### maxf

Maximum of two floats.

### clampf

Clamp float to the inclusive range [min_value, max_value].

### lerp

Linear interpolation between a and b by t in [0,1].

### hypot

Hypotenuse sqrt(x*x + y*y).

### cbrt

Cube root using Newton's method.

### exp2

2^x computed via e^(x*ln 2).

### sinh

Hyperbolic sine.

### cosh

Hyperbolic cosine.

### tanh

Hyperbolic tangent.

