# os

*Source: `os.scar`*

## Functions

### exec

`exec(string command) -> i64`

Execute a command.

### exec_with_args

`exec_with_args(string command, list[string] args) -> i64`

Execute a command with arguments.

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

`get_args() -> list[string]`

Get the command line arguments.

### read_dir

`read_dir(string path) -> list[string]`

Read the contents of a directory.

### clear

`clear()`

Clear the terminal.

