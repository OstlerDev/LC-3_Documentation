# Lesson 1: Program Instructions - `.ORIG`, `HALT`, `.END`
We'll start with the basic building blocks of any LC-3 program, the `.ORIG`, `HALT`, and `.END` instructions. These instructions are required in starting and stopping your program. If you do not include them, your program will not build/assemble!

I know these are boring to learn first, but bear with me, it's a quick lesson and you can move onto the next one very quickly.

## 1. Starting Your Program: The `.ORIG` Instruction
- **Purpose:** .ORIG stands for "origin" and is used to specify where in memory your program will begin.

- **Usage:** An LC-3 program always starts with `.ORIG x3000`

```assembly
.ORIG x3000
```
- **Explanation:** Think of `.ORIG` as setting the starting point for where your code is stored. Don't worry if you don't understand it right now, you honestly don't need to.

## 2. Stop the program running: The `HALT` Instruction
- **Purpose:** HALT is used to stop the program execution. When the LC-3 simulator reaches this instruction, it will cease executing further instructions.

- **Usage:** Place `HALT` at the point in your program where you want it to stop.

```assembly
HALT
```
- **Explanation:** It's like saying, "Okay, we're done here," to your LC-3 program.

## 3. Ending Your Program: The `.END` Instruction
- **Purpose:** `.END` marks the end of your assembly program. It tells LC-3 where the end of your code file is.

- **Usage:** Always place `.END` as the last line of your program.

```assembly
.END
```

- **Explanation:** You can think of `.END` as the end of your all your code, it tells LC-3 that there's nothing more to read or execute in your program.

## Practice Exercise
We already created an example program inside Section 2.2, please take a look there for example code.

## Reflection
- **Understanding the Structure:** This exercise helps you understand the fundamental structure of an LC-3 assembly program. Although this program doesn’t perform any operations, it's a crucial first step in learning assembly programming.

Congratulations on completing your first lesson! You now know how to start, halt, and end a program in LC-3 assembly language. As simple as these instructions may seem, they are vital for every program you'll write in the future in LC-3