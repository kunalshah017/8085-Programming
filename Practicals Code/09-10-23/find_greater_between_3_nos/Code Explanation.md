# 8085 Program to find greater between 3 numbers

Aim - Three numbers are stored in memory location 2501H, 2502H and 2503H. Write a program to find out the greater number and store the result in memory location 2504H.

| Address | Instruction Name | Opcode  |
| ------- | ---------------- | ------- |
| C000    | LXI H, 2501      | 21      |
| C001    |                  | 01      |
| C002    |                  | 25      |
| C003    | MOV B,M          | 46      |
| C004    | INX H            | 23      |
| C005    | MOV A,M          | 7E      |
| C006    | CMP B            | B8      |
| C007    | JNC C00B         | D2      |
| C008    |                  | 0B      |
| C009    |                  | C0      |
| C00A    | MOV A,B          | 78      |
| C00B    | INX H            | 23      |
| C00C    | CMP M            | BE      |
| C00D    | JNC C011         | D2      |
| C00E    |                  | 11      |
| C00F    |                  | C0      |
| C010    | MOV A,M          | 7E      |
| C011    | STA 2504         | 32      |
| C012    |                  | 04      |
| C013    |                  | 25      |
| C014    | HLT              | 76      |

---
## Input
| Address | Data |
| ------- | -----|
| 2501    | 50   |
| 2502    | 70   |
| 2503    | 60   |


## Output

| Address | Data |
| ------- | -----|
| 2504    | 70   |
