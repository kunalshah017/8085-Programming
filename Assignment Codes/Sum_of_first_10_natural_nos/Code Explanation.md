# 8085 Program to find sum of first 10 natural numbers

Aim - Write an assembly language program to find the sum of a series 1+2+3+....+10 (or sum of first 10 natural numbers). Store the result at 2010 memory address.

| Address | Instruction Name | Opcode  |
| ------- | ---------------- | ------- |
| C000    | MVI A, 00H       | 3E      |
| C001    |                  | 00      |
| C002    | MVI B, 0AH       | 06      |
| C003    |                  | 0A      |
| C004    | ADD B            | 80      |
| C005    | DCR B            | 05      |
| C006    | JNZ C004H        | C2      |
| C007    |                  | 04      |
| C008    |                  | C0      |
| C009    | STA 2010H        | 32      |
| C00A    |                  | 10      |
| C00B    |                  | 20      |
| C00C    | HLT              | 76      |

---
## Input
| Address | Data |
| ------- | -----|


## Output

| Address | Data |
| ------- | -----|
| 2010    | 37   |

