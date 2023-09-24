# 8085 Program to add 2 16 bit numbers

Aim - Add the 16-bit number in memory locations 2501H and 2502H to the 16-bit number in memory locations 2503H and 2504H. The most significant eight bits of the two numbers to be added are in memory locations 2502H and 4004H. Store the result in memory locations 2505H and 2506H with the most significant byte in memory location 2506H.


| Address | Instruction Name | Opcode  |
| ------- | ---------------- | ------- |
| C000    | LHLD 2501H       | 2A 01 25 |
| C003    | XCHG             | EB      |
| C004    | LHLD 2503H       | 2A 03 25 |
| C007    | MOV A, E          | 7B      |
| C008    | ADD L            | 85      |
| C009    | MOV L, A         | 6F      |
| C00A    | MOV A, D         | 7A      |
| C00B    | ADC H            | 8C      |
| C00C    | MOV H, A         | 67      |
| C00D    | SHLD 2505H       | 22 05 25 |
| C010    | HLT              | 76      |


---
## Input
| Address | Data |
| ------- | -----|
| 2501    | 05   |
| 2502    | 03   |
| 2503    | 05   |
| 2504    | 03   |


## Output

| Address | Data |
| ------- | -----|
| 2505    | 0A   |
| 2506    | 06   |
