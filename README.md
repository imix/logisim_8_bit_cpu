# Logisim 8-bit CPU

This is a toy 8-bit CPU written in [logisim evolution](https://github.com/logisim-evolution/logisim-evolution). 

The CPU has two working registers, A and B. A is the automatic target of many operations.

It has a smallish instruction set.

| mnemonic | operation | opcode | description |
| -------- | --------- | ------ | ----------- |
| NOP	| 	| 0000 | no operation |
| LDA Addr	| Addr -> A	| 0x01 | load value from address into Register A |
| LDB Addr	| Addr -> B	| 0x02 | load value from address into Register B |
| STA Addr	| A -> Addr	| 0x03 | store value from Register A into address|
| STB Addr	| B -> Addr	| 0x04 | store value from Register B into addres |
| ADD	| A + B -> A	| 0x05 | Add A and B and store into A|
| SUB	| A - B -> A	| 0x06 | Substract B from A and store into A |
| MUL	| A * B -> A	| 0x07 | Multiply A and B and store into A |
| DIV	| A / B -> A	| 0x08 | Divide A by B and store into A |
| AND	| A & B -> A	| 0x09 | bitwise AND A and B |
| OR	| A | B -> A	| 0x0A | bitwise OR A and B |
| NOT	| NOT A -> A	| 0x0B | bitwise NOT A |
| JMP Addr	| JMP Addr | 0x10 | Unconditional jump to address |
| JPZ Addr	| JMP if zero to Addr | 0x20 | jump if zero bit set |
| HLT	| HALT | 0xff | halt operation |


## Sample programs
In the folder sample\_programs you find some examples. Load them into the RAM and run the simulation.
