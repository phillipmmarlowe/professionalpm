+++
date = 'Dec 3, 2025'
draft = false
title = 'Semi General Physical Design Flow for eFPGA RTL'
tags = ["Phillip Marlowe", "HSC", "FPGA", "ASIC", "Physical Design"]
categories = ["projects"]
+++

During my masters, I assisted in the development of a semi-general, semi-automated physical design flow for ASIC/FPGA that has been used to produce multiple real designs, including an N8 K4 4×4 FPGA, an N2 K4 8×8 FPGA, and several smaller blocks such as individual FPGA tiles, CLBs, and buffer chains. All of these designs are implemented using open-source process design kits (PDKs). The primary target has been the ASAP7 PDK from ASU, while the FreePDK45 (Free45nm) from NC State has been used to produce a CLB in an alternative process node. This project focuses on building a reusable, configurable back-end flow that can take FPGA-style RTL through to layout on modern open PDKs, enabling rapid experimentation with different architectures and technology nodes.

{{< figure
    src="https://phillipmmarlowe.github.io/professionalpm/images/image1.png"
    alt="FPGA Physical Design Flow"
    title="N8 K4 4x4 FPGA GDSII"
    caption="Image of a Top-down flow produced N8 K4 4x4 FPGA GDSII"
    width="300"
    class="about-figure"
>}}
