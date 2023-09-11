# 8085 Program to add  2 Numbers stored at 2 Memory Locations

Aim - Two numbers are stored at memory location `2017H` and `2018H`, add them and store result at `2019H`

| Address | Instruction Name | Opcode  |
| ------- | ---------------- | ------- |
| C000    | LDA 2017H        | 3A 17 20|
| C003    | MOV B, A         | 47      |
| C004    | LDA 2018H        | 3A 18 20|
| C007    | ADD B            | 80      |
| C008    | STA 2019H        | 32 19 20|
| C00B    | HLT              | 76      |


---
## Input
| Address | Data |
| ------- | -----|
| 2017    | 04   |
| 2018    | 04   |


## Output

| Address | Data |
| ------- | -----|
| 2019    | 08   |
