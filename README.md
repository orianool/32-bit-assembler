# 10-bit-assembler
School project - 10 bit assembler

The goal of this project was to create a compiler that translates source code written in an imaginary assembley language \(with syntex symilar to MIPS Assembley language\) into machine language.

The machine is also imaginary and has a 10 bit architecture. The istructions are of course 10 bit long and the machine has 8 general purpose registers and 256 "cells" of memory \(each "cell" is 10 bits\).
This architecture supports the basic instructions you would expect (add, sub, jmp, ect...) and can use the following addressing methods:
  1. Immediate addressing
  2. Direct addressing
  3. Register addressing
  4. Struct access addressing \(add explanation\)

The program outputs 3 file in base 32 \(define the base\):
  1. \(output_file\).as - the complete program with the data defined within it after the last istruction.
  2. \(output_file\).ent - contains the name and content of symbols defined as entries.
  3. \(output_file\).ext - contains the name of symbols defined as external and addresses of instructions referring to the symbol.

# usage
./assembler file1 file2...
do not add file extension.
