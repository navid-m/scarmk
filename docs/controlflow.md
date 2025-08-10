# Control Flow

Control flow is trivial and easy to get a handle on in Scar, is it is much like Python or any other imperative programming language.

### if

```python
var x = 10

if x == 10:
    print "Will print."
```

### while

```python
while x < 10:
    print "Do some action..."
```

### for .. to

```
for i = 0 to 10:
    print "%d" | i
```

### for |options|

```
for i32 x = 1; x < 20; x += 2:
    print "odd: %d" | x
```

### foreach

Currently only applicable to iteration through map types, for example a type of `map[string: string]`

```
map[int: string] x = [1: "hello", 2: "world"]

put!(x, 3, "new value")
put!(y, "new key", "new value")
put!(y, "2", "some other value value")

foreach (string z in x.values):
    print "Value: %s" | z
```

### reverse

```
reverse for i = 10 to 1:
    print "Countdown: %d" | i
```

### break

```
reverse for i = 10 to 1:
    if i == 5:
        break
    print "Countdown: %d" | i
```

### continue

```
reverse for i = 10 to 1:
    if i == 5:
        continue
    print "Countdown: %d" | i
```

### try, catch and throw

```
try:
    some_risky_thing()
catch:
    throw 1
```
