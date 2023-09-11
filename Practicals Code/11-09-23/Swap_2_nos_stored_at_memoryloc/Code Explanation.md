# 8085 Program to Swap 2 Numbers stored at 2 Memory Locations

Aim - Two numbers are stored at memory location `2017H` and `2018H`, swap them

| Address | Instruction Name | Opcode  |
| ------- | ---------------- | ------- |
| C000    | LDA 2017H        | 3A 17 20|
| C003    | MOV B, A         | 47      |
| C004    | LDA 2018H        | 3A 18 20|
| C007    | STA 2017H        | 32 17 20|
| C00A    | MOV A, B         | 78      |
| C00B    | STA 2018H        | 32 18 20|
| C00E    | HLT              | 76      |

---
## Input
| Address | Data |
| ------- | -----|
| 2017    | 11   |
| 2018    | 22   |


## Output

| Address | Data |
| ------- | -----|
| 2017    | 22   |
| 2018    | 11   |

