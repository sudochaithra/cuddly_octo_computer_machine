Hardware Specs: 
1. Registers: 8 general-purpose 8-bit registers (R0 to R7, encoded as0x00 to 0x07).
2. Memory: 256 bytes of RAM (addresses 0x00 to 0xFF, 0 to 255).
3.Program Counter (pc): 8-bit pointer starting at 0x00.
Instruction Set (opcodes):
0x00 (HALT): 1 byte total ([0x00]). Stops execution and prints the Octocat register dump.
0x01 (LOAD): 3 byte total ([0x01] [REG] [VAL]). Loads a literal byte(0-255) into REG.
0x02 (ADD): 3 bytes total ([0x02] [REG_A] [REG_B]). Adds REG_B into REG_A (REG_A = REG_A + REG_B).
0x03 (SUB): 3 bytes total ([0x03] [REG_A] [REG_B]). Subtracts REG_B from REG_A (REG_A = REG_A - REG_B).
0x04 (JMP): 2 bytes total ([0x04] [ADDR]). Sets pc directly to ADDR.
