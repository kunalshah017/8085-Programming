# 8085 Program to store data to memory location

Aim - 8085 program to store data in memory location 2050H

| Address | Instruction Name | Opcode  |
| ------- | ---------------- | ------- |
| C000    | MVI A, 50        | 3E      |
| C001    | STA 2050         | 32      |
| C002    |                  | 50      |
| C003    |                  | 20      |
| C004    | HLT              | 76      |

---
## Input
| Address | Data |
| ------- | -----|
| REG A   | 50   |


## Output

| Address | Data |
| ------- | -----|
| 2050    | 50   |
