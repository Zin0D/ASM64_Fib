# Fibonacci in Assembly

A cool and fast Fibonacci sequence generator written in **x86-64 Assembly**! This program takes user input for the number of iterations and prints the corresponding Fibonacci sequence. 

## Features:
- **64-bit Fibonacci**: Computes Fibonacci numbers using 64-bit registers.
- **User Input**: Accepts the number of Fibonacci iterations via standard input.
- **Fast**: Direct assembly language implementation for speed and efficiency.
- **No dependencies**: Pure assembly, just run on an x86-64 system.

## How It Works:
1. **User Input**: The program asks for the number of Fibonacci iterations to calculate.
2. **Computation**: The program calculates Fibonacci numbers using efficient 64-bit register operations.
3. **Output**: The Fibonacci sequence is printed to the terminal, one number per line.

## Instructions to Run:

### Requirements:
- x86-64 system
- `nasm` assembler
- `ld` (for linking)

### Steps:
1. **Assemble the code**:
   nasm -f elf64 FIB.s
   ld -o Fib FIB.o -lc --dynamic-linker /lib64/ld-linux-x86-64.so.2
   ./Fib 
