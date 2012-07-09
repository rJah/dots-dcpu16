# Introduction

dots is a simple OS for DCPU 16. It can be built using 0x10c DevKit
(http://0x10c-devkit.com/). The source uses its macro capabilities heavily.

The solution is divided into several sub-projects. There will definitely be more
of these, but for now they are:
* Core - The kernel proper
* StackCall - Calling convention definitioins
* Std - Math, String, Mem functions
* Hal - Simple Hardware Abstraction Layer
* InitProc - Initializes the Hardware


# Project structure

The solution file is dots-v0.0.3-dcpu16.10csln, which contains all of the
sub-projects. Each project is located in its seperate sub-folder.








