---
title: "Tensor Processing Unit ASIC"
excerpt: "An implementation of Google's TPUv1 from RTL to GDSII on a low-power ASIC.<br/><img src='/images/padviewofchip.png' width='500'>"
collection: portfolio
---

[GitHub Repo](https://github.com/anthonyhermez/Google-TPU)<br>
[Go back](../portfolio/)

Design Description
------
I designed my own Tensor Processing Unit from RTL to GDSII on a 476µm by 476µm ASIC using TSMC 65nm technology nodes and Cadence/Synopsys flows. I architected the TPU from scratch, creating my own 5-instruction CISC ISA, built an Assembler in Python, and microarchitected all blocks of the RTL, including an NxN weight-stationary systolic array to perform matrix multiplication in SystemVerilog. I went through the entire ASIC design flow, including Functional Verification, Synthesis, Floor Planning, Power Planning, P&R, Pad Placement, and Signoff. The chip is getting manufactured, to which I will perform post-silicon validation of the chip.<br>
**Skills:** _ASIC Design Flow, RTL Design, Verification, SystemVerilog, Genus, Innovus, Tempus, Voltus, Virtuoso, Verdi_

Deliverables
------
- [Design Document](../files/Full-stack%20TPU%20Implementation%20and%20Integration%20Analysis%20of%20FPGA%20vs.%20ASIC.docx.pdf)
_See the GitHub for more system and microarchitectural details._

Citations
------
- [Google TPUv1](../files/TPU%20ISCA%202017.pdf)
- [Understanding Matrix Multiplication on a Weight-Stationary Systolic Architecture](https://telesens.co/2018/07/30/systolic-architectures/)