---
title: "The Patt Processor"
excerpt: "A custom structural Verilog implementation of the x86.<br/><img src='/images/pipeline_summary.jfif' width='500'>"
collection: portfolio
---

[Go back](../)

Design Description
------
Named after our professor Dr. Yale Patt, my friends and I designed a [custom x86 implementation](/files/x86_uarch_sp26.pdf) from architectural specification to functional verifiation using only structural gate primatives in three months. Our processor features a 6-stage pipeline with a Banked I-Cache, Next-line Prefetcher, G-Share Branch Predictor, Non-blocking Writeback D-Cache, Non-Stalling Writeback Stage, Double-Clocked Address and Data Bus, and an advanced D-Cache replacement policy. Moreover, we interface I/O devices such as a Keyboard and DMA, and support interrupt and exception handling.<br><br>
**Skills:** _Microarchitecture, Computer Architecture, RTL Design, Verification_

Deliverables
------
- [Design Document](../../files/x86_uarch_sp26.pdf)

Project Specification
------
- [Course Website](https://users.ece.utexas.edu/~patt/26s.382N/)


Acknowledgments
------
Thank you to Jiwoo and Roy for the countless hours spent to make this project happen!.