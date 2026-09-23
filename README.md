# Modern C++ Hello World

A minimal C++23 application built with CMake.

## Requirements

- CMake 3.20 or newer
- A C++23-compatible compiler with support for `<print>`

## Build and run

```sh
cmake -S . -B build
cmake --build build
./build/hello_world
```

On Windows, run `.\build\Debug\hello_world.exe` when using a multi-configuration generator.
