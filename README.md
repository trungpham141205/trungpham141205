<h1 align="center">Hi 👋, I'm Trung Pham</h1>

<h3 align="center">
Digital IC Design Intern | RTL Design | RISC-V CPU | AXI5 | FPGA
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
- Practicing **self-checking testbenches**, directed testing, waveform debugging, and timing-aware verification
- Running RTL simulation and debugging with **Synopsys VCS**, **QuestaSim**, and **ModelSim**
- Working on **AXI5-Full** interface logic, burst transaction behavior, and DMA-oriented SoC integration
- Prototyping digital systems on FPGA using **Quartus**, **SignalTap**, and related FPGA toolchains

---

## Technical Skills

| Area | Skills |
|---|---|
| **HDL & RTL Design** | Verilog, SystemVerilog, synthesizable RTL, FSM, datapath/control design |
| **Computer Architecture & SoC** | RISC-V RV32I, single-cycle CPU, AXI5-based integration, memory-mapped I/O, DMA IP, accelerator integration |
| **Verification & Simulation** | Self-checking testbench, directed testing, functional simulation, waveform debugging, Synopsys VCS, QuestaSim, ModelSim |
| **FPGA Implementation** | Intel Quartus Prime, SignalTap, Gowin IDE, DE1-SoC, Tang Primer 20K Lite |
| **Programming & Tools** | C/C++, Python, Tcl basics, Git, Visual Studio Code, Vim, Linux |

---

## Featured RTL Work

### RISC-V RV32I Single-Cycle CPU on FPGA

A modular 32-bit single-cycle RISC-V processor supporting an RV32I-compatible instruction subset, implemented from RTL design and functional verification to FPGA synthesis and on-board validation.

Key work:

- Designed the Program Counter, instruction decoder, control unit, register file, ALU, immediate generator, branch/jump logic, load/store unit, instruction/data memories, and write-back path
- Implemented R-, I-, S-, B-, U-, and J-type instruction formats
- Supported arithmetic, logical, shift, comparison, branch, jump, and byte/halfword/word memory-access operations
- Verified individual modules and the complete CPU using directed and self-checking testbenches
- Loaded compiled programs through `program.hex` and validated CPU behavior on DE1-SoC FPGA using SignalTap
- Achieved timing closure with no timing violations, +3.923 ns worst setup slack, and 62.2 MHz estimated Fmax at a 50 MHz system clock

---

### AXI-Based SoC Integration with CNN Accelerator

A memory-mapped SoC integration project where a custom RISC-V CPU configures, starts, monitors, and retrieves results from a CNN hardware accelerator.

Key work:

- Implemented AXI-style VALID/READY channel handshake behavior
- Kept address, data, and control payloads stable until handshake completion
- Added CPU stall control to preserve PC, register-file state, address, and transaction data during multi-cycle bus transfers
- Built a software-controlled accelerator flow using `program.hex`, control registers, completion polling, result readback, and RAM storage
- Verified end-to-end CNN accelerator execution flow across multiple input samples

---

### AXI5-Full Interface & DMA IP Integration

Ongoing RTL development for upgrading the processor memory interface toward AXI5-Full and preparing the SoC architecture for DMA-based data movement.

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
