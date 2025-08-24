# os

*Source: `os.scar`*

## Functions

### exec

`exec(string command) -> i64`

Execute a command.

### exit

`exit(i64 code)`

Exit the program.

### cwd

`cwd() -> char*`

Get the current working directory.

### chdir

`chdir(string path) -> int`

Change the current working directory.

### homedir

`homedir() -> char*`

Get the home directory.

### get_env

`get_env(string name) -> char*`

Get an environment variable.

### tempdir

`tempdir() -> char*`

Get the temporary directory.

### get_args

`get_args() -> collections::StringArrayList`

Get the command line arguments.

### clear

`clear()`

Clear the terminal.

