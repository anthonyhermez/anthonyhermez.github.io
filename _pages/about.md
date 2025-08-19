---
permalink: /
title: "Welcome to my homepage!"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<img src="../images/IMG_4041.jpg" alt="My Avatar" style="float: right; margin-left: 15px; margin-bottom: 10px; width: 350px;">

👨🏻‍💻 I’m a final year M.S. ECE student at [The University of Texas at Austin](https://www.utexas.edu/).

🔬 In undergrad, I double majored in [ECE](https://www.ece.utexas.edu/) and [Mathematics](https://math.utexas.edu/) with a minor in [Computational Engineering](https://oden.utexas.edu/).

📚 I’m currently working as an the head TA for [Intro to Embedded Systems](https://users.ece.utexas.edu/~valvano/mspm0/). Last summer I completed a FPGA internship at [Applied Research Laboratories](https://www.arlut.utexas.edu/).

🎻 I also play cello for the [UT University Orchestra](https://music.utexas.edu/ensembles/university-orchestra) and am learning Arabic and Spanish.

What I do
======
I am passionate about advancing the frontiers of computer architecture, with a deep interest in hardware/software co-design and the development of hardware accelerators. My approach is grounded in mathematical rigor and driven by a fascination with high-performance computing. I enjoy dissecting complex systems to identify performance bottlenecks and architecting optimized hardware solutions that align tightly with algorithmic structures. My goal is to contribute to the design of next-generation computing platforms that are not only computationally powerful but also efficient and scalable, enabling transformative capabilities in scientific computing, machine learning, and beyond.

Current Projects
------
<img src="../images/padviewofchip.png" alt="My Avatar" style="float: right; margin-left: 15px; margin-bottom: 10px; width: 300px;">
**Pipelined Polynomial HW Accelerator**<br>
I am developing a Python script that generates RTL in Verilog or VHDL for any polynomial function. The design leverages a numerical algorithm called _Horner's Method_ in a pipelined fashion. The FoM for the generated designs is numerical accuracy, so each pipeline stage scales with the output of the previous stage to avoid truncation precision loss.

**Google TPU ASIC**<br>
Inspired by [Google TPUv1](../files/TPU%20ISCA%202017.pdf), I designed my own Tensor Processing Unit on a 476µm by 476µm ASIC using TSMC 65nm technology nodes and Cadence/Synopsys flows. I architected the TPU from scratch, creating my own 5-instruction CISC ISA, built an assembler in Python, and microarchitected all blocks of the RTL, including an NxN weight-stationary systolic array to perform matrix multiplication in SystemVerilog. I went through the entire ASIC design flow, including functional verification, synthesis, floor planning, power planning, P&R, pad placement, and signoff. I will perform post-silicon validation of the chip after the chip is manufactured.

Selected Experience
------
<img src="../images/IMG_4044.jpg" alt="My Avatar" style="float: right; margin-left: 15px; margin-bottom: 10px; width: 300px;">
**FPGA Engineer Intern**, _Applied Research Laboratories_<br>
Designed RTL in VHDL for accelerating signal processing and digital communication applications.

**SoC Design Verification Engineer Intern**, _Apple_<br>
Developed a complete UVM testbench for a distributed MMU IP in SystemVerilog.

**Validation Engineer Intern**, _Texas Instruments_<br>
Designed and simulated an analog circuit that isolates high voltage from a temperature forcing unit.

**Embedded Software Engineer Intern**, _Applied Research Laboratories_<br>
Programmed firmware in C++ for a high-frequency radio-link simulator to interface with analog and digital attenuators.
