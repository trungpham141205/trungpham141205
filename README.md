<h1 align="center">Hi 👋, I'm Trung Pham</h1>

<h3 align="center">
Digital IC Design | RTL Design | Computer Architecture
</h3>

---

## About Me

I'm an Electronics and Telecommunications Engineering student at **VNUHCM - University of Science**, focused on building clean, verifiable, and timing-aware digital hardware — from RTL simulation to FPGA prototyping. Open to **Master's research opportunities in Microelectronics / IC Design**, as well as **RTL/hardware engineering roles**.

🔭 **Currently building:** a RISC-V-based Secure SoC (AXI4/AXI5 interconnect, 6 cryptographic accelerators, CNN inference engine) for two FPGA design competitions — Oct 2026.

---

## Technical Skills

### HDL, Verification & EDA Tools
<p>
  <img src="https://img.shields.io/badge/-Verilog-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-SystemVerilog-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-Synopsys%20VCS-purple?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-QuestaSim-green?style=for-the-badge" />
</p>

### Architecture & Security
<p>
  <img src="https://img.shields.io/badge/-RISC--V%20RV32I-black?style=for-the-badge&logo=riscv&logoColor=white" />
  <img src="https://img.shields.io/badge/-AMBA%20AXI4%2FAXI5-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-Crypto%20Accelerators%20(AES%C2%B7SHA--256%C2%B7ASCON%C2%B7PRESENT%C2%B7ChaCha20%C2%B7PRINCE)-red?style=for-the-badge" />
</p>

### FPGA & Boards
<p>
  <img src="https://img.shields.io/badge/-Intel%20Quartus-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-SignalTap-yellow?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-DE1--SoC%20(Cyclone%20V)-green?style=for-the-badge" />
</p>

### Programming & Environment
<p>
  <img src="https://img.shields.io/badge/-C%2FC%2B%2B-blue?style=for-the-badge&logo=cplusplus&logoColor=white" />
  <img src="https://img.shields.io/badge/-Python-yellow?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/-Red%20Hat%20(RHEL)-cc0000?style=for-the-badge&logo=redhat&logoColor=white" />
  <img src="https://img.shields.io/badge/-Vim-019733?style=for-the-badge&logo=vim&logoColor=white" />
</p>

🕒 Also practicing timing closure: setup/hold analysis, SDF back-annotation, and gate-level netlist (GLN) simulation.

---

## Featured Projects

### [RISC-V RV32I Single-Cycle CPU on FPGA](https://github.com/trungpham141205/RV32I_Single_Cycle.git)
A modular 32-bit processor implementing the RV32I instruction subset, developed from RTL design to on-board validation.
* **Architecture:** Custom datapath supporting R, I, S, B, U, and J-type instructions.
* **Verification:** Validated via self-checking testbenches and compiled `program.hex` execution.
* **Implementation:** Deployed on DE1-SoC FPGA achieving +3.923 ns worst setup slack and 62.2 MHz Fmax with zero timing violations.

### [AXI5-Lite SoC Integration with CNN Accelerator](https://github.com/trungpham141205/SoC-RV32I-CNN-.git)
A custom hardware-software environment where a RISC-V CPU manages a CNN hardware accelerator.
* **Protocol:** Implemented AXI5-Lite channels (AW, W, B, AR, R) with strict VALID/READY handshakes.
* **Control Logic:** Developed precise CPU stall control to preserve register states during multi-cycle memory-mapped transactions.
* **Flow:** End-to-end software execution including START control, completion polling, and result readback.

---
