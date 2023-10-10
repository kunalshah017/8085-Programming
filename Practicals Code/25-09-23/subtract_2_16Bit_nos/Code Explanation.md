# 8085 Program to subtract two 16-bit numbers

Aim - Write an assembly language program to subtract two 16-bit numbers stored at memory location 2501H and 2503H. Store the result at memory location 2505H and 2506H.


| Address | Instruction Name | Opcode  |
| ------- | ---------------- | ------- |
| C000    | LHLD 2501H       | 2A 01 25 |
| C003    | XCHG             | EB      |
| C004    | LHLD 2503H       | 2A 03 25 |
| C007    | MOV A, E          | 7B      |
| C008    | SUB L            | 95      |
| C009    | MOV L, A         | 6F      |
| C00A    | MOV A, D         | 7A      |
| C00B    | SBB H            | 9D      |
| C00C    | MOV H, A         | 67      |
| C00D    | SHLD 2505H       | 22 05 25 |
| C010    | HLT              | 76      |


---
## Input
| Address | Data |
| ------- | -----|
| 2501    | 10   |
| 2502    | 00   |
| 2503    | 04   |
| 2504    | 00   |

## Output

| Address | Data |
| ------- | -----|
| 2505    | 05   |
| 2506    | 00   |

