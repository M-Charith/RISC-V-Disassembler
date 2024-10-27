# RISC-V-Disassembler

This project was completed as part of the **CS2233** course under the guidance of **Dr. Rajesh Kedia**. The goal of the project is to develop a **RISC-V Disassembler**, which converts RISC-V machine code into human-readable RISC-V instructions.

## Author

- [@M-Charith](https://github.com/M-Charith)

## Tech Stack

- **Command Line**: C++

## Features
- Converts an 8-digit HEX RISC-V machine code into its equivalent RISC-V assembly instruction.
- Designed to take inputs from the terminal, with a `-1` flag to terminate input intake.

## Prerequisites

Before running the project, ensure that you have the `g++` compiler installed by running:

```bash
g++ --version
```
## Installation and Usage
### 1. Clone the Repository
To begin, clone this repository to your local system:

```bash
git clone https://github.com/M-Charith/RISC-V-Disassembler.git
```

### 2. Navigate to the Project Folder
```bash
cd RISC-V-Disassembler
```

### 3. Compile the Code
Use `g++` to compile the source code:

```bash
g++ -o Disassembler disassembler.cpp
```

### 4. Run the Application
Execute the compiled application:

```bash
./Disassembler
```


### Example Usage

**Input:**
```
007201b3
00720863
00c0006f
00533623
100004b7
00c50493
```

**Output:**
```
0: (L7): add x3, x4, x7 
4: beq x4, x7, L1
8: jal x0, L1
c: sd x5, 12(x6)
10: lui x9, 0x10000
14: (L1): addi x9, x10, 12
```


The application accepts input directly from the terminal. Provide each instruction as an 8-digit hexadecimal code, with each on a new line. Conclude the input with `-1` to signal the end of input.

## Documentation
For detailed information about the project, see the [ES21BTECH11021_Disassembler_Report.pdf] file.

--- 
