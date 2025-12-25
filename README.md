
# NAND2TETRISPROJECTMANAGEMENTPART2-Project-9

## Project 9 – Basic Operating System (OS I)

**Project Code:** PROJECT09
**Course:** Build a Modern Computer from First Principles (Nand2Tetris Part II)
**Institution:** Hebrew University of Jerusalem

---

## Overview

Project 9 introduces the first phase of the **Nand2Tetris Operating System**, providing **basic OS-level routines** for programs running on the Hack platform. These routines handle memory access, stack operations, and simple I/O, forming the foundation for user programs and system-level functionality in later projects.

---

## Objectives

* Implement **memory access routines** (`push`/`pop`) for different segments.
* Implement **stack arithmetic operations**.
* Implement **basic screen and keyboard routines**.
* Test OS routines using **VM Emulator** and **hardware simulator**.

---

## Folder Structure

```
Project9/
│── README.md
│── lib/
│   └── Sys.vm
│── test/
│   ├── MemoryTest.vm
│   ├── StackTest.vm
│   └── ScreenTest.vm
│── docs/
│   └── OSI_Guide.pdf
```

---

## Getting Started

### Step 1: Load OS Library

The `Sys.vm` file contains the core OS routines. Ensure it is available in the same directory as your program.

### Step 2: Run Test Programs

1. Open the **VM Emulator**.
2. Load `MemoryTest.vm` or `StackTest.vm`.
3. Observe the correct operation of push/pop and stack commands.

### Step 3: Verify Output

* Screen routines in `ScreenTest.vm` should display patterns on the Hardware Simulator.
* Keyboard input routines can be tested using simple interactive programs.

---

## Supported Features

### Memory Access

* `constant`, `local`, `argument`, `this`, `that`, `pointer`, `temp`, `static` segments
* `push` and `pop` operations

### Stack Operations

* Arithmetic: `add`, `sub`, `neg`
* Logical: `and`, `or`, `not`
* Comparison: `eq`, `gt`, `lt`

### I/O Routines

* Screen manipulation: `Sys.Screen`
* Keyboard input: `Sys.Keyboard`

### Example

**Memory Test (`MemoryTest.vm`):**

```vm
push constant 10
pop local 0
push constant 20
pop argument 0
push local 0
push argument 0
add
```

Expected output: top of stack = 30

---

## Notes

* Project 9 routines **lay the foundation for Project 10**, which implements advanced OS features.
* Ensure all programs include the `Sys.vm` library to run correctly.
* Testing should cover **stack operations, memory access, and I/O routines** thoroughly.

---

## Author

**Aravind Kumar GS**
Email: `aravindkumar06062006@gmail.com`
---

## License

Educational purposes only. Do not distribute or claim as your own work.
