# Understanding Assembly Language Instruction Format
## The Basics of LC-3 Assembly Language
- **What Are Instructions?:** In assembly language, an instruction is a command that tells the computer what to do. Each instruction in LC-3 consists of a few key components that define its operation.
## Structure of an LC-3 Instruction
Basic Format: An LC-3 instruction typically follows this format:

```assembly
OPCODE PARAMETERS ; COMMENTS
```
Let's break down what each part means:

- **OPCODE:** The operation code (opcode) specifies the instrution/operation to be performed (e.g., `AND`, `ADD`, `LD`).
- **PARAMETERS:** These are the inputs for the operation, such as registers or values.
- **COMMENTS:** Anything following a semicolon (;) is a comment, ignored by the assembler but useful for human readers.

## Understanding Opcodes and Parameters
- **Opcodes:** Opcodes are the heart of your instructions. Each opcode has a specific purpose, like adding numbers (ADD) or loading data from memory (LD).

- **PARAMETERS:** Parameters can be numbers, registers, constants, or memory addresses. The amount and type of parameters depend on the opcode. For example, the `ADD` opcode has 3 parameters 

```assembly
ADD R2, R2, #1
```

## Writing a Simple Instruction
Here's a simple example:

```assembly
ADD R2, R2, #1 ; Increment the value in R2 by 1
```
This instruction adds 1 to the value in register R1.

## Comments for Readability
- **Using Comments:** Comments are crucial for making your code readable. They do not affect the program's execution but provide explanations and context for human readers. Always use comments to explain the logic behind your code.

## Practice
- **Try It Out:** Modify the ADD instruction to increase by 2 instead of 1. Don't worry about making a complete program yet, this is just to get comfortable with the format.

