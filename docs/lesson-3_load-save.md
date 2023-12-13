# Lesson 3: Load/Save Instructions and Understanding Labels - LD, ST, and Labels
Welcome to Lesson 3, where we'll cover LD (Load) and ST (Store) instructions in LC-3 assembly language, along with an introduction to what Labels are and how they're used.

## 1. Understanding Labels
- **What Are Labels?:** Labels are basically variables. 

- **Advanced Explanation:** To be specific a Label points to a location in memory that a variable is stored at. Labels are very flexible and can point to pretty much anywhere in code, making using them extremely powerful. In the later lessons you will start to see what else we can do with Labels.

- **Defining a Label:** You can define a label by simply writing it at the start of a line followed by a value (or an instruction, but more on that later).

```assembly
DATA_LABEL .FILL #25  ; Defines a label DATA_LABEL with the value 25
```
- **Using Labels:** Labels are particularly useful with LD and ST instructions for referring to variables without needing to bother with knowing their memory locations. They are basically variables like in higher level languages.

## 2. Loading Data: The LD Instruction
- **Purpose:** The LD instruction loads data from memory into a register.
- **Usage:** 
```assembly
LD DST, LABEL
```

- **DST** the register you want to load the variable into.
- **LABEL** the variable we are loading

```assembly
; Loads the value from memory location labeled DATA_LABEL into R1
LD R1, DATA_LABEL ; R1 now is #25
```

## 3. Storing Data: The ST Instruction
- **Purpose:** The ST instruction stores data from a register into memory.
- **Usage:** 
```assembly
ST SRC, LABEL
```

- **SRC**: the data you want to save to the variable
- **LABEL**: the variable we are saving to

```assembly
ST R3, DATA_LABEL  ; Stores the value in R3 into the memory location labeled STORAGE_LABEL
```

## Practice Exercise
Load, Modify, and Store: Write a program that uses `LD` to load a variable into a register, modifies the register (e.g., add 2), and then uses `ST` to store the register into the variable.

## Reflection
Importance of Load/Store and Labels: Learning how to use `LD` and `ST`, along with understanding labels, is crucial. These are the tools that allow you to interact with variables, which is a great way to reduce some of the headache while writing Assembly code! Using variables will save you from having to manage your registers extrememly carefully, since you will not need to worry about your register getting overwritten (though, more on that later).

Congratulations on completing Lesson 3! You have now mastered the basic data handling instructions in LC-3 assembly language and taken an important step in understanding how to effectively structure your programs.