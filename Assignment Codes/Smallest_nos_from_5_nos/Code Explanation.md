# 8085 Program to find smallest number from 5 numbers

Aim - Write an assembly language program to find the smallest number in a block of 5 numbers.Store the smallest number in memory location 2056.

| Address | Instruction Name | Opcode  |
| ------- | ---------------- | ------- |
| C000    | MVI C, 04H       | 0E      |
| C001    |                  | 04      |
| C002    | LXI H, 2051H     | 21      |
| C003    |                  | 51      |
| C004    |                  | 20      |
| C005    | MOV A, M         | 7E      |
| C006    | INX H            | 23      |
| C007    | CMP M            | BA      |
| C008    | JC C00CH         | DA      |
| C009    |                  | 0C      |
| C00A    |                  | C0      |
| C00B    | MOV A, M         | 7E      |
| C00C    | DCR C            | 0D      |
| C00D    | JNZ C006H        | C2      |
| C00E    |                  | 06      |
| C00F    |                  | C0      |
| C010    | STA 2056H        | 32      |
| C011    |                  | 56      |
| C012    |                  | 20      |
| C013    | HLT              | 76      |

## Input
| Address | Data |
| ------- | -----|
| 2051    | 03   |
| 2052    | 02   |
| 2053    | 04   |
| 2054    | 01   |
| 2055    | 05   |

## Output

| Address | Data |
| ------- | -----|
| 2056    | 01   |


