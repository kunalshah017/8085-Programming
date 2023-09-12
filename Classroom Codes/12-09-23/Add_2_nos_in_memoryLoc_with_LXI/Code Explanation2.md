# 8085 Program to add 2 Numbers stored at memory location

Aim - two 8 bit numbers stored in memory location 2501H and 2504H. Store the result in memory location 2506H. use LXI instruction.

| Address | Instruction Name | Opcode  |
| ------- | ---------------- | ------- |
| C000    | LXI H, 2501H     | 21 01 25 |
| C003    | MOV A, M         | 7E      |
| C004    | LXI H, 2504H     | 21 04 25 |
| C007    | ADD M            | 86      |
| C008    | STA 2506H        | 32 06 25 |
| C00B    | HLT              | 76      |

---
## Input
| Address | Data |
| ------- | -----|
| 2501    | 05   |
| 2504    | 03   |

## Output

| Address | Data |
| ------- | -----|
| 2506    | 08   |
