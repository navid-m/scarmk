# Comments

Comments are denoted with the `#` character.

Like this:

```
## This function returns back what it gets because it's cool
fn cool_function(i32 back) -> i32:
    return back
```

Docstrings are always denoted with double hashes, and are above the function signature, directly above it. No newlines.

As usual, comments should describe why the code does what it does rather than what it does.

In addition to single-line comments, you can use docstrings to provide more detailed explanations for functions, modules, or complex code blocks. Docstrings help other developers understand the purpose and usage of your code, making maintenance and collaboration easier. Always place docstrings immediately above the relevant code, and keep them concise yet informative.

Importantly, `//` and `/* */` syntax is invalid. Comments are strictly denoted with `#`.
