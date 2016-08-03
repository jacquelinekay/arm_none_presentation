~45 minute presentation

# Intro to Embedded Systems

## What is an embedded system and why do we care? (5-10 min)

How should we categorize embedded systems?

Application?

Hardware?
Limited RAM and storage space?
Lack of certain peripherals?

Software?
Instruction set architecture?
Operating system?

Examples
Intel Curie
Jetson TK1/TX1
Raspberry Pi
Beaglebone
STM32


## Embedded development environments (5-10 min)
IDE
Often wraps editor, debugger, and bootloader
Often coupled with the hardware

e.g. Arduino, which is historically a GUI and an abstraction layer for Atmel/ATmega family
STM provides an IDE for development

No-IDE

Cross-compilers:
arm-none-eabi-* GNU toolchain
clang
ARM has a proprietary tool called "armclang" which, I believe, is a proprietary LLVM-based counterpart to the GNU toolchain

OpenOCD (On-chip debugger) <3

Give some examples of:

looking objdumps, elf, etc.
looking at debugger output

## Getting started with OpenOCD and the ARM GNU toolchain (5 min)


## Take a step back: A vision for software (5 min)
But what are we going to put on our board now that we know how to develop for it?
IoT: I kind of hate the name, but the idea is cool
Small hardware components interconnecting data streams originating from many places and sources of data

We need software interoperability and a way to pass messages between machines
I like saving lines of code! Cross-platform software is great
How do we write it? And how different is it to write code on constrained, no-OS environments?

My project: a super-portable implementation of the RTPS standard

## Code (20min)

### Associative vs. sequential: time vs. space tradeoffs

### Multithreading
No <thread>

### Sockets

### Serialization


