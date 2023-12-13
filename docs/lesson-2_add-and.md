# Lesson 2: Arithmetic Instructions - `ADD` and `AND`
In this lesson, we focus on two essential arithmetic operations in LC-3 assembly language: `ADD` and `AND`. These instructions allow you to perform mathematical and logical operations.

## 1. Adding Values: The `ADD` Instruction
- **Purpose:** The `ADD` instruction is used for addition, either between two registers or a register and a constant.

- **Usage:** 
  - Add two registers: `ADD DST, SRC1, SRC2`
  - Add a register and a constant: `ADD DST, SRC, #CONST`

```assembly
ADD R1, R2, R3   ; Adds R2 and R3, stores result in R1
ADD R1, R1, #5   ; Adds 5 to R1, stores result in R1
```

- **Explanation:** `ADD` is your go-to instruction for summing values in LC-3, similar to the plus sign (+) in math.
## 2. Logical `AND` Operation: The `AND` Instruction
- **Purpose:** `AND` allows you to check if a specific bit, or set of bits are set inside a register.

- **Usage:**
    - AND two registers: AND DST, SRC1, SRC2
    - AND a register and a constant: AND DST, SRC, #CONST

```assembly
; Assume R1 = #1
AND R2, R1, #1   ; Set the first bit in R1 into R2
; In this case R2 would be set to 1
```
In a slightly more complex example that is essentially the same, we check the rightmost bit of R1 and since 3 in binary ends with `11`, R2 gets set to `1` (the rightmost bit of R1)
```assembly
; Assume R1 = #3
AND R2, R1, #1   ; Set the first bit in R1 into R2
; In this case R2 would still be 1
```

- **Explanation:** The AND instruction is like a filter, keeping only the bits set in both operands.

## Practice Exercise
- **Simple Addition Program:** Write a program that uses `ADD` to add R1 and R2 to each other.
- **Logical Operation:** Use `AND` to check the second bit of R1!

## Reflection
- **Arithmetic and Logical Operations:** These basic operations are fundamental for building more complex programs in assembly language.

Congratulations on completing Lesson 2! You have now learned to perform basic arithmetic and logical operations in LC-3 assembly language, paving the way to more advanced concepts! I promise at some point this will become interesting to you.
