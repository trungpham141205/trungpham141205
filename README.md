<h1 align="center">Hi 👋, I'm Trung Pham</h1>

<h3 align="center">
Frontend Digital IC Design | RTL Design | FPGA
</h3>

---

## About Me

I am an Electronics and Telecommunications Engineering student at  
**VNUHCM - University of Science**, focusing on **RTL/Digital IC Design**, **functional verification**, **FPGA implementation**, **RISC-V processor architecture**, and **AXI-based SoC integration**.

My engineering interests are centered around building clean, verifiable, and timing-aware digital hardware systems from RTL simulation to FPGA prototype.

---

## Current Focus

- Designing synthesizable RTL using **Verilog** and **SystemVerilog**
- Developing and verifying a **RISC-V RV32I single-cycle CPU**
- Practicing **self-checking testbench**, directed testing, waveform debugging, and timing-aware verification
- Running RTL simulation and debugging with **Synopsys VCS**, **QuestaSim**, and **ModelSim**
- Working with **AXI5-Lite / AXI5-Full** interface logic, VALID/READY handshake, burst transactions, and DMA-oriented SoC integration
- Prototyping digital systems on FPGA using **Intel Quartus Prime**, **SignalTap**, and related FPGA toolchains

---

## Technical Skills

### HDL & RTL Design

<p>
  <img src="https://img.shields.io/badge/-Verilog-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-SystemVerilog-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-Synthesizable%20RTL-blueviolet?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-FSM-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-Datapath%2FControl-purple?style=for-the-badge" />
</p>

### Verification & Simulation

<p>
  <img src="https://img.shields.io/badge/-Self--Checking%20Testbench-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-Directed%20Testing-yellow?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-Functional%20Simulation-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-Waveform%20Debugging-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-Synopsys%20VCS-purple?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-QuestaSim-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-ModelSim-lightgrey?style=for-the-badge" />
</p>

### Computer Architecture & SoC

<p>
  <img src="https://img.shields.io/badge/-RISC--V%20RV32I-black?style=for-the-badge&logo=riscv&logoColor=white" />
  <img src="https://img.shields.io/badge/-Single--Cycle%20CPU-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-AXI5--Lite-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-AXI5--Full-blueviolet?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-Memory--Mapped%20I%2FO-lightgrey?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-DMA%20IP-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-Accelerator%20Integration-red?style=for-the-badge" />
</p>

### FPGA Implementation

<p>
  <img src="https://img.shields.io/badge/-Intel%20Quartus%20Prime-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-SignalTap-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-Gowin%20IDE-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-DE1--SoC-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-Tang%20Primer%2020K%20Lite-purple?style=for-the-badge" />
</p>

### Programming & Tools

<p>
  <img src="https://img.shields.io/badge/-C%2FC%2B%2B-blue?style=for-the-badge&logo=cplusplus&logoColor=white" />
  <img src="https://img.shields.io/badge/-Python-yellow?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/-Tcl-lightgrey?style=for-the-badge" />
  <img src="https://img.shields.io/badge/-Git-red?style=for-the-badge&logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/-VS%20Code-blue?style=for-the-badge&logo=visualstudiocode&logoColor=white" />
  <img src="https://img.shields.io/badge/-Vim-green?style=for-the-badge&logo=vim&logoColor=white" />
  <img src="https://img.shields.io/badge/-Linux-black?style=for-the-badge&logo=linux&logoColor=white" />
</p>

---

## Featured RTL Work

### RISC-V RV32I Single-Cycle CPU on FPGA

A modular 32-bit single-cycle RISC-V processor supporting an RV32I-compatible instruction subset, implemented from RTL design and functional verification to FPGA synthesis and on-board validation.

Key work:

- Designed the Program Counter, instruction decoder, control unit, register file, ALU, immediate generator, branch/jump logic, load/store unit, instruction/data memories, and write-back path
- Implemented R-, I-, S-, B-, U-, and J-type instruction formats
- Supported arithmetic, logical, shift, signed/unsigned comparison, branch, jump, and byte/halfword/word memory-access operations
- Verified individual modules and the complete CPU using directed and self-checking testbenches
- Loaded compiled programs through `program.hex` and validated PC, instruction, RegWrite, destination-register, and write-back behavior on DE1-SoC FPGA using SignalTap
- Achieved timing closure with no timing violations, +3.923 ns worst setup slack, 62.2 MHz estimated Fmax, and CPI = 1 at a 50 MHz system clock

---

### AXI5-Lite SoC Integration with CNN Accelerator

An AXI5-Lite-based SoC integration project where a custom RISC-V CPU configures, starts, monitors, and retrieves results from a CNN hardware accelerator through memory-mapped software operations.

Key work:

- Implemented the AW, W, B, AR, and R channels using VALID/READY handshake control
- Kept transaction payloads stable until handshake completion
- Added CPU stall control to preserve PC, register-file state, address, and transaction data throughout multi-cycle AXI transfers
- Built a software-controlled accelerator flow using `program.hex`, START control register write, completion polling, classification readback, and RAM storage
- Verified end-to-end CNN accelerator execution flow across multiple input samples

---

### AXI5-Full Interface & DMA IP Integration

Ongoing RTL development for upgrading the processor memory interface from AXI5-Lite to AXI5-Full and preparing the SoC architecture for DMA-based data movement.

Current work:

- Designing separate write and read transaction FSMs across AW/W/B and AR/R channels
- Adding AXI5-Full transaction fields including ID, LEN, SIZE, BURST, and LAST
- Supporting initial single-beat 32-bit transfers, one in-flight transaction, and no out-of-order transactions
- Implementing transaction-wide CPU stall control, aligned address generation, byte-lane WDATA shifting, WSTRB generation, and signed/unsigned load-data extension
- Verifying VALID/READY behavior under slave backpressure and checking payload stability until handshake completion
- Preparing the AXI interconnect, address map, and memory-mapped control path for DMA IP integration

---

### RTL Timing Verification Practice

Additional RTL practice focused on functional correctness, timing behavior, and waveform-based debugging.

Included designs and verification topics:

- 4-bit Ripple Carry Adder
- 8-bit SIPO Shift Register
- D Flip-Flop with timing checks
- Setup/Hold violation testbench
- Recovery/Removal timing verification
- Worst-case timing path analysis
- RTL simulation with Synopsys VCS / QuestaSim / ModelSim
- Waveform-based debugging
