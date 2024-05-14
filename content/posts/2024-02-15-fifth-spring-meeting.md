+++
title = '5th Spring 2024 Meeting'
date = 2024-02-15T10:54:17-05:00
draft = false
summary = 'club meeting, downsides of using dev c++, dev c++ alternatives'
tags = ['meeting', 'Dev-C++', 'C-C++', 'IDE', 'VS Code'] 
+++

***

# Overview

- Attendance
- Don't Use Dev-C++
- Next Week

***

## Attendance

- Abu Shettima
- Christian Messmer
- Jeremiah Neff
- Jonathan Buckel
- Paul Shriner
- Matthew Williams

## Don't Use Dev-C++

### What is Dev-C++?

Dev C++ is an IDE for the C and C++ programming languages. It was originally released in 1998 and has had several forks since. This IDE is recommended by the professors on campus.

### Benefits of Dev-C++

...

### Why is it bad?

It is VERY outdated. This IDE is lacking:
- Version control integration
- Syntax highlighting
- Meaningful extensions
- Comprenhensive code completion 
- Features and refinements from newer GCC compilers

### Dev-C++ is LITERALLY broken!

There is an "undo" bug. When you hit the undo/redo buttons multiple times, your code can become corrupted. Large sections of your source code will be deleted! Additionally, the IDE will sometimes just crash at random.

### Stop using Dev-C++

It is not safe to rely on Dev-C++ when completing programming assignments. Luckily, there are plenty of alternatives that can be used instead.

### Alternative: VS Code

[VS Code](https://code.visualstudio.com/download) is not an IDE, but it is way more functional than Dev-C++ and works for school assignments. It may seem daunting at first, but it is really not bad to set up. It is very extensible, and can be used for numerous programming languages. For those that do not wish to support Microsoft, there is an alternative called [VSCodium](https://vscodium.com/).

### Installing a C/C++ compiler

A C/C++ compiler will need to be manually acquired to use with VS Code. One such option is through [MSYS2](https://www.msys2.org/). Once downloaded, run ```pacman –Syu``` to update the base packages. Then, run ```pacman -S --needed base-devel mingw-w64-ucrt-x86_64-toolchain``` to install GCC and other utilities. Finally, add the MSYS2 bin directory to the path. More details can be found [here](https://code.visualstudio.com/docs/cpp/config-mingw).

### Using a Makefile

The easiest way to compile C/C++ programs is with a Makefile. To install make using MSYS2, run ```pacman --S make```. You can use a premade Makefile, or follow this [tutorial](https://makefiletutorial.com/) to create a Makefile.

### Need an IDE?

* [Visual Studio](https://visualstudio.microsoft.com/downloads/)
* [Jetbrains CLion](https://www.jetbrains.com/clion/) 
    * This IDE is paid, but it can be accessed for free with the GitHub student pack.
* [Code::Blocks](https://www.codeblocks.org/downloads/) 
    * This has a lot of the same problems as Dev-C++, but it does not delete your code!

## Next Week

Next week, we will be having a meeting on Thursday at 11 AM in Eberly 342. Have a resume ready for February 29th, in which there will be a resume workshop.
