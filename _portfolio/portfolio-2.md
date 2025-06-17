---
title: "Ordinary Differential Equation HW Accelerator"
excerpt: "ODE HW Accelerator on a Zynq UltraScale+ FPGA interfaced with physics application.<br/><img src='/images/ode_accelerator_vivado.png' width='500'>"
collection: portfolio
---

[Go back](../)

Design Description
------
A high-speed single-precision floating-point ODE differential equation HW accelerator on the Zynq UltraScale+ MPSoC tailored to interface with a 3-dimensional n-body physics simulation.<br><br>
**Skills:** _Verilog, Xilinx Vivado, FPGAs, Linux Kernel Modules, Embedded C, Numerical Analysis_

Technical Details
------
- **Numerical Algorithm:** Of the many ODE algorithms available, we chose to use the 4th-order Runge-Kutta (RK4) method for two main reasons: 1) This algorithm has 4th-order numerical stability, meaning if the step size is decreased by a factor of 2, the solution is 16-times more accurate. This allowed us to use larger step sizes while still achieving accurate results. 2) Across all scientific literature, no one has ever implemented RK4 on an FPGA. We wanted a challenge :)
- **Single-Precision FP:** Due to resource limitations and the desire for more solvers, single-precision FP was chosen over double-precision. This significantly reduced the number of DSP slices used per solver. The FP units were Xilinx IP and used AXI Stream protocol.
- **Pipelined Architecture:** To further decrease the number of DSP slices used per solver, the accelerator design pipelined its resources. The bottleneck of the design was calculating the acceleration vector, so we leveraged some calculation optimizations, such as implementing the fast inverse square-root algorithm into a 4-cycle operation. All of these optimizations decreased the cycle count by 16 cycles from the original design.
- **User Application:** We connected multiple accelerators to a terminal application running the n-body simulation. Due to our resource optimizations, we could run up to 35 particles in parallel.

Deliverables
------
- [Final Presentation Slides](../../files/ode_accelerator_slides.pptx)

Citations
------
- [Runge-Kutta Methods](https://en.wikipedia.org/wiki/Runge%E2%80%93Kutta_methods)
- Sauer, Timothy. Numerical Analysis. 3rd ed., Pearson, 2019.

Acknowledgments
------
Thank you Francisco for helping with the physics application software.
