# Variables

The type of variables can be inferred with `var`, however this is only if the type of the variable is obvious by observing the right hand side of the expression.

## Type Inference with `var`

When you use `var`, the compiler tries to figure out the variable's type based on what you assign to it. This is called _type inference_. It makes your code cleaner and easier to read, but only works when the type is clear.

For example, this will work:

```
var calc = new Calculator()
```

Here, the compiler knows that `calc` is of type `Calculator` because you are creating a new `Calculator` object.

## When Type Inference Fails

This will not:

```
var something = some_thing()
```

If `some_thing()` is a function and its return type is not clear to the compiler (for example, if it returns a generic object or its return type is not specified), the compiler cannot infer the type for `something`. In such cases, you must explicitly specify the type:

```
Thing calc = some_thing()
```

or, if `some_thing()` returns an `int`:

```
int result = some_thing()
```

## Why This Matters

Type inference helps reduce repetition, but it’s important to use it only when the type is obvious. If the type is unclear, your code can become harder to understand and maintain, and the compiler will give you an error.

### Good Example

```
var number = 42;    # Clearly an int
var name = "Alice"; # Clearly a string
```

### Bad Example

```
var data = GetData(); # What type is data? Not clear!
```

In the bad example, unless `GetData()` has a clear return type, it’s better to specify the type explicitly.

## Summary

-  Use `var` when the type is obvious from the right-hand side.
-  If the type is not clear, specify it explicitly to avoid confusion and compiler errors.
