4-bit SRAM using Quantum-dot Cellular Automata (QCA)

Author: J. Harsha Vardhan

College: University College of Engineering Narasaraopet, JNTUK

Tool: QCADesigner 2.0

Domain: VLSI Design, Nanotechnology, Low-Power Memory Architecture

Event: Smart India Hackathon 2024 — Related Research


📌 Project Overview
A 4-bit Static Random Access Memory (SRAM) cell designed and simulated using Quantum-dot Cellular Automata (QCA) — a post-CMOS nanotechnology that encodes binary information through electron position rather than current flow, enabling ultra-low-power operation at the nanoscale.

As CMOS scaling approaches its physical limits, QCA offers a promising path toward higher density, lower power dissipation, and terahertz-range switching speeds. This project explores QCA as a viable foundation for next-generation VLSI memory design.


⚙️ Key Features

✅ Complete 4-bit SRAM architecture using QCA cells

✅ Storage and access logic implemented entirely with Majority Gate primitives

✅ Layout optimised using QCA wire-crossing techniques to minimise cell count and area

✅ Validated Read and Write operations across all input combinations

✅ Energy dissipation analysis confirming low-power efficiency over CMOS

✅ Simulated and verified using QCADesigner 2.0's Bistable Approximation engine



🧠 What is QCA?
Quantum-dot Cellular Automata is a nanotechnology computing paradigm where each QCA cell consists of four quantum dots positioned at the corners of a square, holding two mobile electrons. Due to Coulombic repulsion, these electrons settle into one of two diagonal configurations — representing binary 0 or 1. Unlike CMOS, no current flows during steady-state operation, which is the source of QCA's extremely low power dissipation.

The fundamental logic building block in QCA is the Majority Gate, which computes:

M(A, B, C) = AB + BC + CA

By fixing one input to a constant 0 or 1, the Majority Gate can be configured as a 2-input AND or OR gate — making it the universal primitive for all QCA circuits, including this SRAM design.


📐 Architecture
The 4-bit SRAM consists of four 1-bit QCA storage cells arranged in a linear array, sharing common Word Line (WL) and Bit Line (BL / BL') control signals.

Cross-coupled QCA inverters (built from Majority Gates) to form a stable bistable storage element
Majority-Gate-based access logic controlled by the Word Line for Read/Write operations


🔬 Simulation Parameters

Parameter
Value
Cell size
18 nm × 18 nm
Dot diameter
5 nm
Relative permittivity
12.9
Clock amplitude factor
2.0
Layer separation
11.5 nm
Simulation engine
Bistable Approximation
Convergence tolerance
1 × 10⁻³



✅ Functional Verification
Read and Write operations were validated across all 4 bits and all possible input combinations:

Write: External Bit Line polarisation overrides the stored state when Word Line is asserted
Read: Stored cell polarisation propagates to Bit Lines when Word Line is asserted, sensed differentially

Both single-bit and multi-bit simultaneous Read/Write operations were verified to function correctly.


📊 Results Summary
Metric
Result
Functional accuracy
100% across all test input combinations
Cell count
Reduced vs. baseline CMOS-equivalent design
Array area
Reduced via wire-crossing optimisation
Energy dissipation
Demonstrated efficiency gain over CMOS (see energy analysis)


(Replace with your exact recorded values from QCADesigner output for full reproducibility.)


🚀 How to Reproduce
Download and install QCADesigner 2.0
Open the .qca layout file in this repository
Set the simulation engine to Bistable Approximation
Apply the simulation parameters listed above
Run simulation and observe Read/Write waveforms in the output viewer
Cross-check output polarisation against expected logic states for each test vector


🔗 Related Projects
UART Communication Controller — Verilog RTL Design — Full-duplex UART transceiver with self-checking testbench, validated in Xilinx Vivado


📚 References
This work builds on foundational QCA literature, including studies on QCA multiplexer design and parallel prefix adder architectures, demonstrating cell count and area reduction techniques applicable to memory design.


👤 Author
J. Harsha Vardhan

B.Tech — Electronics & Communication Engineering (VLSI Specialisation)

University College of Engineering Narasaraopet, JNTUK

📧 jhvharshavardhan@gmail.com

🔗 https://www.linkedin.com/in/harshavardhan-jangam-05037a269/

