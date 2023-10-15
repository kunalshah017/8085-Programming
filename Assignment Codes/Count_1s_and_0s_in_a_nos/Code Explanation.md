# 8085 Program to count number of 1's and 0's in a number

Aim - Write assembly language program to find number of 1's and 0's in 8-bit number stored at 2010 memory address. Store the count of 1's at 2011 memory address and count of 0's at 2012 memory address.

| Address | Instruction Name | Opcode  |
| ------- | ---------------- | ------- |
| C000    | LDA 2010H        | 3A      |
| C001    |                  | 10      |
| C002    |                  | 20      |
| C003    | MVI C, 08H       | 0E      |
| C004    |                  | 08      |
| C005    | MVI D, 00H       | 16      |
| C006    |                  | 00      |
| C007    | MVI E, 00H       | 1E      |
| C008    |                  | 00      |
| C009    | RRC              | 0F      |
| C00A    | JNC C011H        | DA      |
| C00B    |                  | 11      |
| C00C    |                  | C0      |
| C00D    | INR E            | 1C      |
| C00E    | JMP C012H        | C3      |
| C00F    |                  | 12      |
| C010    |                  | C0      |
| C011    | INR D            | 14      |
| C012    | DCR C            | 0D      |
| C013    | JNZ C009H        | C2      |
| C014    |                  | 09      |
| C015    |                  | C0      |
| C016    | LXI H, 2011H     | 21      |
| C017    |                  | 11      |
| C018    |                  | 20      |
| C019    | MOV M, E         | 77      |
| C01A    | INX H            | 23      |
| C01B    | MOV M, D         | 72      |
| C01C    | HLT              | 76      | 

---

## Input
| Address | Data |
| ------- | -----|
| 2010    | 70   |

70 = 01110000


## Output

| Address | Data |
| ------- | -----|
| 2011    | 03   |
| 2012    | 05   |
