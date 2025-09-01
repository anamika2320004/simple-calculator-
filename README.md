**Project Overview**

This project implements a 4-bit ALU (Arithmetic Logic Unit) that can perform arithmetic and logical operations on two 4-bit inputs. Users can select the operation using a 3-bit OP code.

**Operations Supported:**

| OP Code | Operation | Description          |
|---------|-----------|--------------------|
| 000     | ADD       | A + B              |
| 001     | SUB       | A - B              |
| 010     | AND       | A & B              |
| 011     | OR        | A \| B             |
| 100     | XOR       | A ^ B              |
| 101     | NOT       | ~A (only A)        |
| 110     | NAND      | ~(A & B)           |
| 111     | NOR       | ~(A \| B)          |

---

## Verilog Files

1. **txt file ** – ALU design and  Testbench  

---
| Time | A    | B    | OP  | RESULT |                                |               |
| ---- | ---- | ---- | --- | ------ | ------------------------------ | ------------- |
| 10   | 0101 | 0011 | 000 | 1000   | (Add: 5 + 3 = 8)               |               |
| 20   | 0101 | 0011 | 001 | 0010   | (Subtract: 5 - 3 = 2)          |               |
| 30   | 0101 | 0011 | 010 | 0001   | (AND: 0101 & 0011 = 0001)      |               |
| 40   | 0101 | 0011 | 011 | 0111   | (OR: 0101                      | 0011 = 0111)  |
| 50   | 0101 | 0011 | 100 | 0110   | (XOR: 0101 ^ 0011 = 0110)      |               |
| 60   | 0101 | 0011 | 101 | 1010   | (NOT A: \~0101 = 1010)         |               |
| 70   | 0101 | 0011 | 110 | 1110   | (NAND: \~(0101 & 0011) = 1110) |               |
| 80   | 0101 | 0011 | 111 | 1000   | (NOR: \~(0101                  | 0011) = 1000) |
Key Features

Supports arithmetic and logical operations.

Uses a 3-bit OP code for operation selection.

Designed for EDA Playground simulation.
