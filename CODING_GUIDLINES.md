# David Angosto coding guidelines

Coding guidelines may depend on the language or languages used, or maybe the target platform.
So, for each case some general specific documentation is given.

## C/C++

Mainly inspired by:

* [Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html)
* [LLVM Coding Standards](https://llvm.org/docs/CodingStandards.html)
* [Guidelines for the use of the C++14 language in critical and safety-related systems](https://www.autosar.org/fileadmin/standards/R22-11/AP/AUTOSAR_RS_CPP14Guidelines.pdf)
* [SEI CERT C Coding Standard](https://wiki.sei.cmu.edu/confluence/display/c/SEI+CERT+C+Coding+Standard)
* [SEI CERT C++ Coding Standard](https://wiki.sei.cmu.edu/confluence/display/cplusplus)
* [C++ Coding Standards and Style Guide](https://ntrs.nasa.gov/api/citations/20080039927/downloads/20080039927.pdf)
* [JOINT STRIKE FIGHTER AIR VEHICLE C++ CODING STANDARDS FOR THE SYSTEM DEVELOPMENT AND DEMONSTRATION PROGRAM](https://www.stroustrup.com/JSF-AV-rules.pdf)
* [The Power of 10: Rules for Developing Safety-Critical Code](https://web.eecs.umich.edu/~imarkov/10rules.pdf)
* [JPL Institutional Coding Standard for the C Programming Language](https://web.archive.org/web/20111015064908/http://lars-lab.jpl.nasa.gov/JPL_Coding_Standard_C.pdf)
* [Embedded C Coding Standard](https://barrgroup.com/sites/default/files/barr_c_coding_standard_2018.pdf)
* [Free RTOS Coding Standard and Style Guide](https://www.freertos.org/FreeRTOS-Coding-Standard-and-Style-Guide.html)
* [Coding Guidelines — Zephyr Project Documentation](https://docs.zephyrproject.org/latest/contribute/coding_guidelines/index.html#coding-guidelines)

### 1. Files and folders

All source files and directories should be camel_case.
Some valid examples are: resource_mananger.h, resource_mananger.c, main.cpp, main.hpp.

* _c++_ source files should be: `\*.cpp`.
* _c++_ header files should be: `\*.hpp`.
* _c_ source files should be: `\*.c`.
* _c_ header files should be: `\*.h`.
* If compatible with build system all source code files should be under `src/`.
* If compatible with build system all header files should be under `src/`.
* If compatible with build system all unit test files should be under `ut/`.
* If compatible with build system all test code should be under `test/`.
* If compatible with build system all documenation should be under `doc/`.
* If compatible with build system all github actions should be under `.github/`.

### 2. Language

* Standard [c++20](https://en.cppreference.com/w/cpp/20) should be used for _c++_.
* Standard [c17](https://en.cppreference.com/w/c/17) should be used for _c++_.

* Compile with the most restrictive compiler options possible, suchas -pedantic-errors or -Wall for gcc.


### 3. Comments
* Prefer C Style comments, `/**/`, over C++ style.
* All Doxygen documentation should be in the header file unless it is static for a translation unit then it should be

### 4. Fromatting

### 5. Naming

### 6. Naming

### 7. General rules

* Headers file should have a inclusion guard



## Verilog
TBD.

## ADA
TBD.

## rust
TBD.

---
Davang