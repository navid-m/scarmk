# Home

Scar is a programming language designed for ease of use in terms of concurrent programming.
It has a focus on simplicity and performance, making it suitable for a wide range of applications.

## Getting Started

To get started with Scar, you can install it from the [GitHub releases page](https://github.com/navid-m/scar/releases)

-  Extract the downloaded archive.
-  Add the `scar` executable to your system's PATH.
-  Verify the installation by running `scar --version` in your terminal.
-  The VSCode extension can be found [here](https://marketplace.visualstudio.com/items?itemName=NavidM.scar).

See also [Installation Details](#Installation Details) for setup instructions.

## Installation Details

For memory management and garbage collection, Scar uses the BDWGC, which is a concurrent mark-and-sweep garbage collector. GC is optional.

It must be installed on the host system if not running Windows, in which case it is included with the distribution by default.

## First Program

```
parallel for i = 0 to 10:
   print "%d" | i
```

You will notice that when running the code, the output is not in order, as the iterations are executed concurrently.
