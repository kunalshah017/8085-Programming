# 8085 Program to swap two numbers stored in memory location

Aim - 8085 program to swap two numbers stored in memory location 2050H and 2051H

| Address | Instruction Name | Opcode  |
| ------- | ---------------- | ------- |
| C000    | LXI H, 2050      | 21      |
| C001    |                  | 50      |
| C002    |                  | 20      |
| C003    | MOV C,M          | 4E      |
| C004    | INX H            | 23      |
| C005    | MOV B,M          | 46      |
| C006    | MOV A,C          | 79      |    
| C007    | MOV C,B          | 4F      |
| C008    | MOV B,A          | 47      |
| C009    | MOV M,B          | 70      |
| C00A    | DCX H            | 2B      |
| C00B    | MOV M,C          | 71      |
| C00C    | HLT              | 76      |

---
## Input
| Address | Data |
| ------- | -----|
| 2050    | 50   |
| 2051    | 70   |


## Output

| Address | Data |
| ------- | -----|
| 2050    | 70   |
| 2051    | 50   |
