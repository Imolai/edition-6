# My Notes

## Compilation

Clang++ and g++ does not support using modules on:

- Ubuntu 24.04.1 LTS: clang++ v18.1.3; g++ v13.2.0 and
- Termux v0.118.1: clang++ v19.1.2.

Therefore `import std` and `std::println()` have been replaced.

Files:

- [Examples/Ch01/01_HelloWorld/01_helloworld.cpp](Examples/Ch01/01_HelloWorld/01_helloworld.cpp)
- [Examples/Ch01/01_HelloWorld/CMakeLists.txt](Examples/Ch01/01_HelloWorld/CMakeLists.txt)
