# 8085 Program to add 2 Numbers 1 stored in Register and 1 stored at Memory Location

Aim - One number is stored in register `B` and another is stored at memory location `2017H`, add them and store result at `2018H`

| Address | Instruction Name | Opcode  |
| ------- | ---------------- | ------- |
| C000    | LDA 2017H       | 3A 17 20   |
| C002    | MVI B 04H       | 06 04   |
| C004    | ADD B            | 80     |
| C006    | STA 2018H        | 32 18 20|
| C009    | HLT              | 76      |

---
## Input
| Address | Data |
| ------- | -----|
| 2017    | 04   |

## Output

| Address | Data |
| ------- | -----|
| 2018    | 08   |
