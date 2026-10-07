# Andrew Kim

M.S. ECE student at Carnegie Mellon University focused on **RTL design, digital microarchitecture, and FPGA/ASIC development**.

My work has focused on designing and optimizing digital hardware under practical constraints including **timing, power, area, and limited hardware resources**. I am particularly interested in RTL design, computer architecture, hardware accelerators, and low-latency digital systems.

## Selected Work

### [TinyDMA-2C](https://github.com/punchthatface/tinyDMA)

Two-channel SystemVerilog DMA engine developed for TinyTapeout/Sky130.

- Designed register configuration, round-robin scheduling, byte-transfer control, and an SPI PSRAM interface
- Verified RTL with SystemVerilog testbenches and cocotb using Verilator
- Performed FPGA bring-up against physical APS6404 PSRAM
- Optimized the design around a constrained TinyTapeout silicon-area budget
- Completed the TinyTapeout ASIC flow through GDS generation

### STGEMM Accelerator Architecture — Graduate Research

*Source not public*

SystemVerilog microarchitecture research for an energy-efficient GEMM accelerator.

- Explored fixed-cycle low-bit and shared LUT-based datapaths
- Achieved **1.26× geometric-mean latency improvement** with the fixed-cycle design and **1.093× geometric-mean energy improvement** with the LUT-based design across five workloads at 32×32
- Evaluated area, latency, power, and energy using Cadence Genus/Joules
- Automated benchmark execution and result collection with Bash and Python

### Root-of-Trust Hardware Security — CMU 18-632

*Source kept private due to course academic-integrity policies*

Two related SystemVerilog projects covering both timing-driven RTL design and integrated hardware-security architecture.

- **Project 1 — TRNG Statistical Test Engine:** implemented NIST-inspired statistical tests in synthesizable RTL, restructured iterative logic into pipelined datapaths, and achieved **500 MHz timing closure with +99 ps setup slack** using Cadence Genus on ASAP7
- **Project 2 — Root-of-Trust Security Peripheral:** designed a CPU-mapped Root of Trust integrating AES/AES-CTR, PUF, TRNG, PRNG, and primality checking behind a 32-bit register interface
- Implemented shared-resource control for AES, LFSR, and ring-oscillator hardware and developed feature-level and multi-step use-case testbenches

### [Parallel Video Reconstruction](https://github.com/punchthatface/15418-FinalProject)

Parallel video reconstruction from aggressively subsampled frames using C++, OpenMP, and CUDA.

- Implemented bilinear interpolation, iterative stencil refinement, and motion-aware tile classification
- Used Sum of Absolute Differences (SAD) to identify active regions and avoid unnecessary computation
- Built serial, OpenMP, and CUDA implementations
- Evaluated reconstruction quality using MSE, PSNR, and SSIM

## Technical Interests

RTL design · digital microarchitecture · ASIC/FPGA development · computer architecture · hardware accelerators · PPA optimization · timing-driven design

## Languages & Tools

**RTL / Programming:** SystemVerilog, Verilog, C/C++, Python, Bash  
**ASIC / EDA:** Cadence Xcelium, Genus, Joules; Synopsys Design Compiler  
**FPGA / Verification:** Verilator, cocotb, Quartus II, Yosys + nextpnr  
**Platforms:** TinyTapeout/Sky130, Intel/Altera Cyclone V, Lattice ECP5
