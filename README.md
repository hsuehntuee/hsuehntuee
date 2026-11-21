<h1 align="center">Yen-Hung Hsueh 薛晏閎</h1>

<p align="center">
  Electrical Engineering senior at National Taiwan University<br>
  AI accelerators, digital IC design, and the software that models them
</p>

<p align="center">
  <a href="mailto:b12901064@ntu.edu.tw">b12901064@ntu.edu.tw</a>
</p>

## About

I design hardware for machine learning and write the software around it: performance models, compilers and bit-accurate simulators. Before I call a design done, the RTL has to match its software model on every output bit, and where I can get a board or a chip, the measurement has to match too.

I work in two labs at NTU, with Prof. Chia-Hsiang Yang on FPGA and ASIC accelerators and with Prof. Tsung-Te Liu on compute-in-memory chips. I graduate in 2027 and am looking for a summer 2027 internship.

## Research

| Project | What it is |
|---|---|
| On-device VLM accelerator | An inference accelerator for a vision-language model, built from a performance model down to SystemVerilog. The whole image-and-prompt-to-token flow runs bit-exact in RTL simulation. Ongoing, not public yet. |
| [EfficientViT-FPGA-Accelerator](https://github.com/hsuehntuee/EfficientViT-FPGA-Accelerator) | The attention blocks of EfficientViT on a Xilinx VCU128, running inside a PyTorch network over PCIe and matching the integer model on every on-board run. |
| [IBERT-CIM-Inference](https://github.com/hsuehntuee/IBERT-CIM-Inference) | Integer-only BERT inference prepared for a 28 nm compute-in-memory chip. A pretrained BERT now runs end to end on that chip, close to its floating-point accuracy. |

## Chips and processors

| Project | What it is |
|---|---|
| [Binary-Transformer-ASIC](https://github.com/hsuehntuee/Binary-Transformer-ASIC) | A binary-weight Transformer accelerator taped out in 0.18 µm by a team of three, trained so that the software model and the RTL agree bit for bit. |
| [RV32-Pipelined-Processor](https://github.com/hsuehntuee/RV32-Pipelined-Processor) | A six-stage RISC-V core with caches, compressed instructions and branch prediction, built by a team of three. |

## Software

| Project | What it is |
|---|---|
| [Polaris](https://github.com/hsuehntuee/polaris) | An offline voice assistant for Taipei's City Pass app, with a small language model running on the phone's NPU. 2nd place, 2026 Taipei Fall Codefest. |
| [RTL-To-Graph](https://github.com/Ekstaxy/RTL-To-Graph) | A tool that turns Verilog into architecture, state-machine and timing diagrams. I lead the RTL-extraction layer and the integration in a team of three. |
| [pdf-tool](https://github.com/hsuehntuee/pdf-tool) | A self-hosted PDF toolbox that processes files in memory. |

Each repository's README has the measured results, the architecture and how to run it.

## Background

- B.S. in Electrical Engineering, National Taiwan University, expected 2027. GPA 4.16/4.3.
- Research intern at Academia Sinica (CITI), summer 2025, on diffusion models for scannable video QR codes. First author of a manuscript under revision.
- Teaching assistant for Machine Learning (Prof. Hsuan-Tien Lin) and for NTUEE Cornerstone.
- NSTC Undergraduate Research Grant, 2026. Third Prize and Best Popularity Award, NTUEE Undergraduate Project Award, 2026, for a real-time FPGA target-tracking system.

## Tools

SystemVerilog and Verilog with Synopsys VCS, Design Compiler and PrimeTime; Vivado for FPGA work; Calibre for DRC and LVS. Python, C/C++ and Rust. PyTorch for quantization-aware training and bit-accurate integer models.
