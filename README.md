# ˗ˏˋ ★ ˎˊ˗ CUDDLY OCTO COMPUTER MACHINE



 **8-BIT VIRTUAL CPU EMULATOR & CUSTOM BYTECODE ASSEMBLER IN C**

<br>`WSL` `GCC` `Git` `Bash` `Vim` `tmux` `C` `Python 3` `Bash` `Custom Assembly` `Fetch-Decode-Execute Cycle` `Registers & RAM` `Bytecode & Opcodes` `Binary File I/O` `Memory Bounds Checking` `Linux CLI`



<tt>INTRO</tt> 

 * **Cuddly:** so its just friendly, or innocent.

 * **Octo:** Eight tentacles (a nod to GitHub's Octocat mascot), an 8-bit CPU/ emulator.

 * **Computer Machine:** A dead-simple virtual machine.



<tt>REFERENCES</tt> 

 * **CS50X** weeks 1-5 (C fundamentals)

 * **Beej's Guide to C Programming** (quick lookup)



<tt>APPROACH</tt>

 * Set up Linux terminal, `git`, and `vim`/`tmux`. Write `build.sh` to compile a starter `main.c` with `gcc -Wall -Wextra` and run it.

 * After CS50x Weeks 1–2, create 8 registers (`uint8_t reg`), 256 bytes of RAM, and a program counter (`pc`).

 * Hardcode a program that adds two numbers and prints the registers.

 * After CS50x Weeks 3–4 (pointers & file I/O), upgrade the VM to read raw `.bin` files from disk into RAM without recompiling C.

 * Write a 20-line Python assembler (`octo_asm.py`) to turn `LOAD R0, 5` / `ADD R0, R1` into hex bytes.

 * Print an ASCII Octocat register dump on `HALT`.

 * Test bad code and out-of-bounds memory to learn how C fails.



<tt>STRUCTURE</tt>

```text

cuddly_octo_computer_machine/

├── src/main.c # Virtual CPU core

├── tools/octo_asm.py # Text-to-bytecode assembler

├── examples/add.asm # Sample test program

├── build.sh # gcc compile script

└── README.md

```



<tt>RUN</tt>

```bash

./build.sh

python3 tools/octo_asm.py examples/add.asm out.bin

./octo_vm out.bin

```



[dipping already; go to Tactical RnG](https://github.com/sudochaithra/tactical-rng)

