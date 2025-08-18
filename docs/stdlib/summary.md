# Scar Programming Language - Agent Guide

## Overview
Scar is an in-development systems programming language compiler written in Go that transpiles Scar code to C and compiles it. Features parallelism constructs, optional GC, and immutability focus.

## Build/Test Commands
- Build compiler: `go build` or `build.cmd` (Windows)
- Run tests: `go test -v ./...` 
- Run single test: `go test -v -run TestName`
- Compile .scar file: `scar.exe filename` (creates filename.exe)
- With GC: `scar.exe -gc filename`
- Show C output: `scar.exe -c filename`

## Architecture
- `main.go` - Compiler entry point, handles CLI flags, orchestrates compilation pipeline
- `lexer/` - Parsing and validation of Scar source code to AST
- `renderer/` - C code generation from AST
- `preprocessor/` - Source-level macro processing  
- `tests/` - Test files organized by category (prims/, progs/, oop_tests/, etc.)
- `.scar` files transpile to C, then compile with clang/gcc

## Code Style
- Go: Standard Go formatting, camelCase functions, exported types start with capitals
- Scar language: snake_case variables, colon syntax for blocks, explicit types
- Error handling: Return validation errors from lexer, log.Fatal for critical failures
- Comments: Use `//` for Go code documentation when complex
