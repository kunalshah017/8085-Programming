# 8085 Program to add 2 Numbers stored in Registers

Aim - Two numbers are stored in registers `A` and `B`, add them and store answer at memory location `2050H`

| Address | Instruction Name | Opcode  |
| ------- | ---------------- | ------- |
| C000    | MVI A, 05H       | 3E 05   |
| C002    | MVI B, 06H       | 06 06   |
| C004    | ADD B            | 80      |
| C006    | STA 2050H        | 32 50 20|
| C009    | HLT              | 76      |

---

## Output

| Address | Data |
| ------- | -----|
| 2050    | 0B   |
