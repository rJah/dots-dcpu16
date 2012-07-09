# Introduction

dots is a simple OS for DCPU 16. It can be built using 0x10c DevKit
(http://0x10c-devkit.com/). The source uses its macro capabilities heavily.

## Project structure

The solution file is dots-v0.0.3-dcpu16.10csln, which contains all of the
sub-projects. Each project is located in its seperate sub-folder.

There will definitely be more sub-projects, but for now they are:
* Core - The kernel proper and entry point
* StackCall - Calling convention definitioins
* Std - Math, String, Mem functions
* Hal - Simple Hardware Abstraction Layer
* InitProc - Initializes the Hardware

These are not complete yet, they are being added to as needed (mostly copying
and fixing code, from a prevoius implementation).


## Project goals

dots originally got started years ago as a hobby OS project for the x86 and
later moved to amd64, but lately I haven't had the time (or will) to keep
working on it (maybe someday in the future). But I really needed something
low-level to keep the blood flowing, so I decided to see what I can do in pure
assembly on a 16 bit machine I never saw before.

The aim of this project is to have fun and learn things :) Operating systems
are a very interesting topic (to me, at least). Also, I have never done a
full scale project in assembly, so now is my chance.


# InitProc

Currently InitProc initializes Video, Clock, Keyboard and RTC (see below), but
the handlers don't do anything yet.

## Friendly Real Time Clock

Friendly RTC is my (very simple) device plugin for 0x10c DevKit IDE:
A Real Time Clock. It's not necessary for dots to operate, I just didn't remove
the code. I will probably make it available on GitHub when I have fully decided
on the functionality and implemented it.









