# SimpleDumper

Writing simple dumper 4fun for Windows (x86-64). Dumper uses capstone framework to disassembly code of OEP and let user confirm that it is really it. Testing this dumper against UPX currently.
Tested on Windows 7 (6.1.7601 SP1) with GCC 7.3.0 and CMake 3.14.7.

Project is under development !

## How to compile
You gonna need CMake and MinGW (tested) or MSVC (should work)

Compile on Windows with MinGW compiler

```
git clone --recurse-submodules https://github.com/domin568/SimpleDumper
mkdir build
cd build
cmake -G "MinGW Makefiles" ..
mingw32-make
```

## Usage

```
SimpleDumper <exe> <out exe> [OEP]
```
You can provide OEP by yourself and just dump the process. If you do not provide it then dumper gonna try to find OEP on its own by dynamic approach.

## Visual presentation 

![](screen.png) 

