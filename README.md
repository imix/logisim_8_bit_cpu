# Logisim 8-bit CPU

This is a toy 8-bit CPU written in [logisim evolution](https://github.com/logisim-evolution/logisim-evolution). 

The CPU has two working registers, A and B. A is the automatic target of many operations.

It has a smallish instruction set.

| mnemonic | operation | opcode |
| ------- | --------- | --------------------- |
| NOP	| 	| 0000 |
| LDA Addr	| Addr -> A	| 0x01 |
| LDB Addr	| Addr -> B	| 0x02 |
| STA Addr	| A -> Addr	| 0x03 |
| STB Addr	| B -> Addr	| 0x04 |
| ADD	| A + B -> A	| 0x05 |
| JMP Addr	| JMP Addr | 0x10 |
| JPZ Addr	| JMP if zero to Addr | 0x20 |
| HLT	| HALT | 0xff |


## Sample programs
In the folder sample\_programs you find some examples. Load them into the RAM and run the simulation.
