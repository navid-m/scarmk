# Classes

Classes are defined like so:

```
pub class Calculator:
    init:
        i32 this.current_value = 0

    fn subtract(i32 x) -> int:
        return this.current_value - x
```

## Instantiating Classes

To create an instance of a class, use the `new` keyword:

```
let calc = new Calculator()
```

You can then call methods on the instance:

```
calc.subtract(5)
```

## Member Variables

Member variables are defined inside the `init` block. They are accessed using `this`:

```
pub class Counter:
    init:
        i32 this.count = 0

    fn increment():
        this.count = this.count + 1
```

## Constructors

The `init` block acts as the constructor and is called when a new instance is created. You can add parameters to initialize member variables:

```
pub class Point:
    init(i32 x, i32 y):
        i32 this.x = x
        i32 this.y = y
```

## Inheritance

Classes can inherit from other classes using the `:` syntax:

```
pub class AdvancedCalculator : Calculator:
    fn multiply(i32 x) -> int:
        return this.current_value * x
```
