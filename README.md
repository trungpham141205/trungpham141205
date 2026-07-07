<h1 align="center">Hi 👋, I'm Trung Pham</h1>

<h3 align="center">
Digital IC Design | RTL Design | Computer Architecture
</h3>

---

## About Me

I am an Electronics and Telecommunications Engineering student at **VNUHCM - University of Science**. My engineering passion lies in building clean, verifiable, and timing-aware digital hardware systems—from RTL simulation to FPGA prototyping. 

Currently, I am actively seeking **Master's degree opportunities in Microelectronics** to further deepen my expertise in computer architecture and IC design.

---

## Current Focus

- Designing synthesizable RTL using **Verilog** and **SystemVerilog**.
- Developing and verifying a **RISC-V RV32I** single-cycle CPU.
- Researching **Secure SoC Architectures**, specifically the integration of encryption modules (AES) with standard AMBA AXI/AHB buses.
- Practicing functional verification (self-checking testbenches, directed testing) and timing-aware debugging.

---

## Technical Skills

### HDL, Verification & EDA Tools
<p>
  <img src="https://img.shields.io/badge/-Verilog-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-SystemVerilog-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-Synopsys%20VCS-purple?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-QuestaSim-green?style=for-the-badge" />
</p>

### Architecture & FPGA
<p>
  <img src="https://img.shields.io/badge/-RISC--V%20RV32I-black?style=for-the-badge&logo=riscv&logoColor=white" />
  <img src="https://img.shields.io/badge/-AMBA%20AXI5-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-Intel%20Quartus-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-SignalTap-yellow?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-DE1--SoC-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-Tang%20Primer%2020K-purple?style=for-the-badge" />
</p>

### Programming & Environment
<p>
  <img src="https://img.shields.io/badge/-C%2FC%2B%2B-blue?style=for-the-badge&logo=cplusplus&logoColor=white" />
  <img src="https://img.shields.io/badge/-Python-yellow?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/-Red%20Hat%20(RHEL)-cc0000?style=for-the-badge&logo=redhat&logoColor=white" />
  <img src="https://img.shields.io/badge/-Vim-019833?style=for-the-badge&logo=neovim&logoColor=white" />
</p>

---

## Featured Projects

### [RISC-V RV32I Single-Cycle CPU on FPGA](#https://github.com/trungpham141205/RV32I_Single_Cycle.git)
A modular 32-bit processor implementing the RV32I instruction subset, developed from RTL design to on-board validation.
* **Architecture:** Custom datapath supporting R, I, S, B, U, and J-type instructions.
* **Verification:** Validated via self-checking testbenches and compiled `program.hex` execution.
* **Implementation:** Deployed on DE1-SoC FPGA achieving +3.923 ns worst setup slack and 62.2 MHz Fmax with zero timing violations.

### [AXI5-Lite SoC Integration with CNN Accelerator](#https://github.com/trungpham141205/SoC-RV32I-CNN-.git)
A custom hardware-software environment where a RISC-V CPU manages a CNN hardware accelerator.
* **Protocol:** Implemented AXI5-Lite channels (AW, W, B, AR, R) with strict VALID/READY handshakes.
* **Control Logic:** Developed precise CPU stall control to preserve register states during multi-cycle memory-mapped transactions.
* **Flow:** End-to-end software execution including START control, completion polling, and result readback.

### [AXI5-Full & DMA IP Integration (WIP)](#link-to-your-repo)
Ongoing upgrade of the SoC memory interface from AXI5-Lite to AXI5-Full.
* **Current State:** Designing separate FSMs for burst transactions and handling AXI5-Full fields (ID, LEN, SIZE, BURST).
* **Goal:** Preparing the memory-mapped control path and AXI interconnect for seamless DMA data movement.
* 
---

## Timing Verification & Debugging Practice
Beyond architecture, I actively practice verifying timing behavior and debugging complex logic setups. My [Verification Practice Repo](#link-to-repo) includes:
* Setup/Hold violation analysis and Recovery/Removal timing verification.
* 4-bit RCA, 8-bit SIPO Shift Register, and timing-aware D Flip-Flops.
* Extensive waveform debugging using Synopsys VCS, QuestaSim, and ModelSim.

---
