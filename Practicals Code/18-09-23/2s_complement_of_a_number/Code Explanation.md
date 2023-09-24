# 8085 Program to give 2's complement of a number

Aim - Write an assembly language program to give 2's complement of a number stored in memory location 2000H. Store the result in memory location 2001H.

| Address | Instruction Name | Opcode  |
| ------- | ---------------- | ------- |
| C000    | LDA 2000H        | 3A 00 20 |
| C003    | CMA              | 2F      |
| C004    | INR A            | 3C      |
| C005    | STA 2001H        | 32 01 20 |
| C008    | HLT              | 76      |

---
## Input
| Address | Data |
| ------- | -----|
| 2000    | 05   |

## Output

| Address | Data |
| ------- | -----|
| 2001    | FB   |

## 2's complement solving 

0 5 > 0000 0101  
1s Complement > 1111 1010  
2s Complement > 1111 1011  
1111 1011 > F B  