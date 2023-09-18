# 8085 Program to add number stored in memory location 2050 to 2059


Aim - Write an assembly language program to add numbers stored from 2050 to 2059 using JNZ loop and store the result at 205F

| Address | Instruction Name | Opcode   |
| ------- | ---------------- | -------- |
| C000    | LXI H, 2050H     | 21 50 20 |
| C003    | MVI C, 10H       |  0E 10   |
| C005    | ADD M            | 86       |
| C006    | DCR C            | 0D       |
| C007    | INX H            | 23       |
| C008    | JNZ C005H        | C2 05 C0 |
| C00B    | STA 205FH        | 32 5F 20 |
| C00E    | HLT              | 76       |


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
| 2958    | 01   |
| 2059    | 01   |


## Output

| Address | Data |
| ------- | -----|
| 205F    | 0A   |
