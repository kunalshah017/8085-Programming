# 8085 Program to add 2 Numbers in memory location

Aim - Write an assembly language program to add two 8 bit numbers stored in memory location 2501H and 2502H. Store the result in memory location 2503H. use LXI instruction.

| Address | Instruction Name | Opcode  |
| ------- | ---------------- | ------- |
| C000    | LXI H, 2501H     | 21 01 25 |
| C003    | MOV A, M         | 7E      |
| C004    | INX H            | 23      |
| C005    | ADD M            | 86      |
| C006    | STA 2503H        | 32 03 25 |
| C009    | HLT              | 76      |


---
## Input
| Address | Data |
| ------- | -----|
| 2501    | 05   |
| 2502    | 03   |


## Output

| Address | Data |
| ------- | -----|
| 2503    | 08   |
