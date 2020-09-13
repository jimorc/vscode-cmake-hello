# vscode-cmake-hello
Simple project to build a program and library in VSCode using CMake. Testing using GoogleTest is included.

CMake is the defacto standard for build systems. It is supported by every IDE that supports C++.
This repository contains the code that was developed in a set of five articles that I wrote about
using "Modern" CMake and Visual Studio Code to create a simple C++ library and application. The
project is further enhanced to create unit tests using Google Test. CMake files are created to
download and build Google Test and to integrate it into the project.

Looking at the code for this repository, you will see that there are three subdirectories in the
root directory. They contain the following:

## part1

part1 contains the C++ and CMake code that corresponds to the code developed in
[Building C++ Applications With CMake and Visual Studio Code](
https://computingonplains.wordpress.com/building-c-applications-with-cmake-and-visual-studio-code/).
In that article, a simple C++ static library and program are created. The CMake directives in the
CMakeLists.txt files required to build the library and program are described.

## shared_libs

shared_libs contains all of the code from part1 and the changes requilred to change the library
from static to shared. The changes are described in
[Building C++ Applications With Visual Studio Code – Creating a Shared Library](
https://computingonplains.wordpress.com/building-c-applications-with-visual-studio-code-creating-a-shared-library/).
An alternative method that works only on Windows using the Visual Studio build tools is described.

## testing

testing contains all of the code from shared_libs plus the changes required to download and build Google Test
and to create unit tests for the library. The code in this folder is used in the remaining three articles:
[Building C++ Applications With Visual Studio Code – Unit Testing With GoogleTest](
https://computingonplains.wordpress.com/building-c-applications-with-visual-studio-code-unit-testing-with-googletest/),
[Building C++ Applications With Visual Studio Code – Saving the Project to Source Control Using git](
https://computingonplains.wordpress.com/building-c-applications-with-visual-studio-code-saving-the-project-to-source-control-using-git/),
and [Building C++ Applications With Visual Studio Code – Porting to Linux](
https://computingonplains.wordpress.com/building-c-applications-with-visual-studio-code-porting-to-linux/).


In addition to these folders, a .gitignore file, which is created in [the article on source control](
https://computingonplains.wordpress.com/building-c-applications-with-visual-studio-code-saving-the-project-to-source-control-using-git/),
is located in the root directory for this repository.

