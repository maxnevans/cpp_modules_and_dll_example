# C++20 Modules example with DLL

This is an example of C++ modules project with DLL.

## 1. Set environment variables if you want to compile with a specific compiler (e.g. clang).
Hint. In powershell:
```bash
$env:CXX="clang++"
$env:CC="clang"
```

## 2. Generate and build the project
```bash
mkdir build
cmake -S . -B build
cmake --build build --target main
```

Hint. If you want clang, use Ninja generator:
```bash
make build
cmake -GNinja -S . -B build
cmake --build build --target main
```

## Current problems
VS Code doesn't support C++ modules. Syntax highlighting is broken.
 
Track the issue: [Github Issue 6302 - Add IntelliSense for C++20 modules importing](https://github.com/microsoft/vscode-cpptools/issues/6302)