# Access Modifiers

A function can be marked `pub` to expose it as an externally accessible API.

```
pub fn some_function():
    print "This function is accessible outside this module/file."
```

```
pub class Calculator:
    init:
        i32 this.currentval = 0
```

These are not accessible:

```
fn internal_function():
    print "This function is only accessible within this module/file."
```

```
class InternalHelper:
    init:
        i32 this.value = 42
```

Functions and classes without the `pub` keyword are private to their module or file by default. This means they cannot be accessed from outside their defining scope.
