# Functions

Functions are defined like so:

```
fn some_function() -> int:
    return 5
```

The function signature immediately describes what the function does.

Arguments are taken as follows:

```
fn add(i32 x, i32 y) -> int:
    return x + y
```

Again, immediately obvious what this does.

## Return Types

The return type is specified after the arrow (`->`). If a function does not return a value, use `void`:

```
fn log_message(msg: str) -> void:
    print(msg)
```

## Custom Return Types

Functions can return multiple values using custom types:

```
fn min_max(a: int, b: int) -> DataContainer:
    if a < b:
        return new DataContainer(a, b)
    else:
        return new DataContainer(b, a)
```
