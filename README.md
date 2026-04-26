# Project README

## Overview
The project is a simple GUI application that demonstrates basic components such as buttons, labels, and progress bars. It supports building for Linux, Windows (using Wine), WebAssembly, and can be built using GCC or Clang.

## Features
- Basic GUI components: buttons, labels, and progress bars.
- Cross-platform support: Linux, Windows (via Wine), and WebAssembly.

## Project Structure
### Prerequisites
- C/C++ Compiler and Debugger (GCC, Clang)
- Make utility
- Standard development tools
- Libraries needed:
  - For Linux: X11, PNG, JPEG
  - For Windows: WINAPI

## Build & Run
The project uses different Makefiles for each platform to build the application.

### Linux
```sh
cd <Project>
make -f Makefile.linux all
```
To run the application:
```sh
make -f Makefile.linux exe
```

### Windows (using Wine)
```sh
cd <Project>
make -f Makefile.wine all
```
To debug the application:
```sh
make -f Makefile.wine debug
```
To run the application:
```sh
make -f Makefile.wine exe
```

### WebAssembly
```sh
cd <Project>
make -f Makefile.web all
```
To execute the application in a web browser:
```sh
make -f Makefile.web exe
```

These steps will build and run the project on each respective platform.