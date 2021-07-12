#**RV32I**

##What is RISC V?
RISC-V is an open standard instruction set architecture based on established reduced instruction set computer principles. Unlike most other ISA designs, the RISC-V ISA is provided under open source licenses that do not require fees to use.
For more reading visit riscv.org

##What is RV32I
RV32I was designed to be sufficient to form a compiler target and to support modern operating
system environments. The ISA was also designed to reduce the hardware required in a minimal implementation. RV32I contains 47 unique instructions, though a simple implementation
might cover the eight SCALL/SBREAK/CSRR* instructions with a single SYSTEM hardware
instruction that always traps and might be able to implement the FENCE and FENCE.I instructions as NOPs, reducing hardware instruction count to 38 total. RV32I can emulate almost
any other ISA extension (except the A extension, which requires additional hardware support for
atomicity).
 Further reading: https://riscv.org/wp-content/uploads/2017/05/riscv-spec-v2.2.pdf

##What is in this repo?
This repo contains the final code written in TL-Verilog that implements a simple RV32I core that runs a pre-programmed assembly program
