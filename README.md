<h1 align="center">Yen-Hung Hsueh 薛晏閎</h1>

<p align="center">
  Electrical Engineering senior at National Taiwan University<br>
  AI accelerators, digital IC design, and the software that models them
</p>

<p align="center">
  <a href="mailto:b12901064@ntu.edu.tw">b12901064@ntu.edu.tw</a>
</p>

## About

I design hardware for machine learning and write the software around it: performance models, compilers and bit-accurate simulators. Before I call a design done, the RTL has to match its software model on every output bit, and where I can get silicon or a board, the measurement has to match too.

I work in two labs at NTU: the Digital Circuits and Systems Lab with Prof. Chia-Hsiang Yang, and the Energy-Efficient Circuits and Systems Lab with Prof. Tsung-Te Liu. I graduate in 2027 and plan to continue to a master's degree in electronics.

## Projects

| Project | What I built | Measured result | Code |
|---|---|---|---|
| On-device VLM accelerator | A W4A8 inference accelerator for Gemma 4 E2B with speculative decoding. I wrote the performance model, the compiler and the SystemVerilog engine. | The image-and-prompt-to-token flow is bit-exact in RTL simulation across 34 self-checking testbenches. | Private, ongoing lab research |
| EfficientViT accelerator on FPGA | The linear-attention blocks of EfficientViT-B1 on a Xilinx VCU128, running inside a PyTorch segmentation network over PCIe. | 8.3x fewer cycles per block across design iterations. 800 on-board runs match two integer models. 4,755 DSPs, timing clean at 62.5 MHz. | Private, lab research |
| BERT on compute-in-memory silicon | Quantization and training that let a pretrained BERT-Medium run end to end on a 28 nm compute-in-memory chip, with a labmate. | 89.9% on SST-2 and 81.5% on MNLI measured on the chip, within 0.5 points of FP32, at 15.7 µJ per token. | Private, lab research |
| Binary-weight Transformer ASIC | A 0.18 µm tape-out by a team of three. I contributed to the RTL and synthesis, ran DRC and LVS, and handled the submission. | Signed off after place-and-route at 100 MHz and 34.8 mW. | Private |
| [Polaris](https://github.com/hsuehntuee/polaris) | An offline voice assistant for Taipei's City Pass app. Gemma 3 270M, fine-tuned into an intent decider, runs on a phone NPU. | 2nd place, 2026 Taipei Fall Codefest. 93.2% accuracy at 63 ms per decision on a 1,027-utterance test set. | Public |
| [RTL-To-Graph](https://github.com/Ekstaxy/RTL-To-Graph) | A tool that turns Verilog into architecture, state-machine and timing diagrams. I lead the RTL-extraction layer and the integration in a team of three. | Funded by the NTU Challengers Program. | Public |
| Pipelined RISC-V core | An RV32 core with instruction and data caches, compressed instructions and a gshare branch predictor, built by a team of three. | Synthesized at a 2.54 ns clock in a 0.13 µm library. Course final project, Digital System Design. | Private |
| [pdf-tool](https://github.com/hsuehntuee/pdf-tool) | A self-hosted PDF toolbox that processes files in memory. | 22 tools, with a guest mode that runs in the browser. | Public |

The lab projects are private because the chips and papers are not public yet. I can walk through any of them in an interview.

## Background

- B.S. in Electrical Engineering, National Taiwan University, expected 2027. GPA 4.16/4.3.
- Research intern at Academia Sinica (CITI) in summer 2025, on diffusion models for scannable video QR codes. First author of a manuscript under revision.
- Teaching assistant for Machine Learning (Prof. Hsuan-Tien Lin) and for NTUEE Cornerstone.
- NSTC Undergraduate Research Grant, 2026. Third Prize and Best Popularity Award, NTUEE Undergraduate Project Award, 2026, for a real-time FPGA target-tracking system.

## Tools

SystemVerilog and Verilog on Synopsys VCS, Design Compiler and PrimeTime; Vivado for FPGA work; Calibre for DRC and LVS. Python, C/C++ and Rust. PyTorch for quantization-aware training, LoRA fine-tuning and bit-accurate integer models.
