+++
title = 'Using VS Code for C/C++'
date = 2024-04-22T10:26:03-04:00
draft = false
summary = 'Guide for developing C/C++ programs using VS Code'
tags = ['guide', 'C-C++', 'VS Code']
+++

***

# Overview
- Introduction
- Installing VS Code
- Downloading a Compiler
- Setting up VS Code
- Setting up the Environment
- Git/GitHub
- Conclusion

***

# Introduction

The C and C++ programming languages are used in several classes at PennWest California. However, the development environment recommended in these classes, Dev-C++, has several problems as detailed in [previous meetings](/posts/2024-02-15-fifth-spring-meeting). The following guide will cover how to set up a development environment for C/C++ using Visual Studio Code (VS Code).

# Installing VS Code

VS Code can be downloaded from their website [here](https://code.visualstudio.com/).

# Downloading a Compiler

VS Code does not come with a compiler for C/C++, you will need to download one yourself. The compiler we will use is GCC/G++. Note that the compiler will be added to your path, meaning it can be used anywhere, even independently of VS Code.

## Windows

For Windows, we will use MSYS2. VS Code has a guide you can follow [here](https://code.visualstudio.com/docs/cpp/config-mingw#_prerequisites). You only need to follow up to and including *Check your MinGW installation*. 

## Linux

On Linux, it's recommended to install GCC/G++ through your package manager. This will vary depending on the distribution. On Fedora and other rpm based distros, you can use the command:

```
sudo dnf install gcc g++ gdb
```

# Setting up VS Code

Within VS Code, the only setup required by this guide is to install the C/C++ extension found [here](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools). You may change VS Code's other settings, themes, and install other extensions per your preferences. A recommended extension for doing group work is Live Share [here](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare), which allows code collaboration (basically like screen sharing).

# Setting up the Environment

There are several ways to compile and run C/C++ programs within VS Code, we will be using a Makefile. As the Makefiles for C and C++ are slightly different, it is recommended to have two separate folders, one for C and one for C++.

## Makefile

[Here](/guide_vscode_cpp_resources/Makefile-c) is a Makefile for C, and [here](/guide_vscode_cpp_resources/Makefile-cpp) is one for C++. These include pipelines for unit testing, but it is not required to use unit testing in this environment. These Makefiles work on both Windows and Linux.

## Creating the Folder Structure

Create a base folder, call it what you want. Inside the folder, create two folders called "src" and "tests". Copy the Makefile you downloaded earlier into the base folder, being sure to rename it to "Makefile". Open the base folder in VS Code, it should look like this:

{{< figure align=center src=/guide_vscode_cpp_resources/folder_view.png >}}

## Using Your Environment

Your main source files will go in the src folder. You must have at least a main.c or main.cpp. Here are the make commands supported by the Makefiles:

* make - Makes the program, rebuilding if needed
* make all - Makes the program, always rebuilds
* make clean - Cleans object files
* make tests - Makes the program from the tests folder (for unit testing)

# Git/GitHub

It is highly recommended to use your environment in conjunction with a version control platform. We will be writing a guide soon for Git/GitHub you can follow.

# Conclusion

This guide was written by PennWest Software Development Club. If you have any questions, feel free to ask in our Discord or at one of our meetings. And be sure to share this guide around!
