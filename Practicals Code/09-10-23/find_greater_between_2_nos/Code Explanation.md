# 8085 Program to find greater between 2 numbers

Aim - Two numbers are stored in memory location 2501H and 2502H. Write a program to find out the greater number and store the result in memory location 2503H.

| Address | Instruction Name | Opcode  |
| ------- | ---------------- | ------- |
| C000    | LXI H, 2501      | 21      |
| C001    |                  | 01      |
| C002    |                  | 25      |
| C003    | MOV C,M          | 4E      |
| C004    | INX H            | 23      |
| C005    | MOV A,M          | 7E      |
| C006    | CMP C            | B9      |
| C007    | JNC C00B         | D2      |
| C008    |                  | 0B      |
| C009    |                  | C0      |
| C00A    | MOV A,C          | 79      |
| C00B    | STA 2503         | 32      |
| C00C    |                  | 03      |
|C00D     |                  | 25      |
| C00E    | HLT              | 76      | 


---
## Input
| Address | Data |
| ------- | -----|
| 2501    | 50   |
| 2502    | 70   |


## Output

| Address | Data |
| ------- | -----|
| 2503    | 70   |
