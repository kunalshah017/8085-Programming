# 8085 Program to add numbers stored in 10 memory locations

Aim - Write an assembly language program to add 10 8 bit numbers stored in memory location 2050H to 2059H. Store the result in memory location 2060H. use JNZ instruction.

| Address | Instruction Name | Opcode  |
| ------- | ---------------- | ------- |
| C000    | LXI H, 2050H     | 21 50 20 |
| C003    | MVI C, 0AH       | 0E 0A   |
| C005    | MOV A, M         | 7E      |
| C006    | ADD M            | 86      |
| C007    | INX H            | 23      |
| C008    | DCR C            | 0D      |
| C009    | JNZ C005         | C2 05 C0 |
| C00C    | STA 2060H        | 32 60 20 |
| C00F    | HLT              | 76      |

---
## Input
| Address | Data |
| ------- | -----|
| 2050    | 01   |
| 2051    | 01   |
| 2052    | 01   |
| 2053    | 01   |
| 2054    | 01   |
| 2055    | 01   |
| 2056    | 01   |
| 2057    | 01   |
| 2058    | 01   |
| 2059    | 01   |


## Output

| Address | Data |
| ------- | -----|
| 2060    | 0A   |
