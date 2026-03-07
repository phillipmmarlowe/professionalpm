+++
title = "TinyTapeout 5 — HLS Leaky Integrate and Fire Neuron"
date = "2023-11-04T00:00:00Z"
draft = false
tags = ["tinytapeout", "asic", "open-source-silicon"]
summary = "TinyTapeout 5 shuttle tapeout: tt_um_hls_lfi."
thumbnail = "https://phillipmmarlowe.github.io/professionalpm/images/tinytapeout5chip.png"
+++

## Overview

For the class ECE210L: Brain Inspired Machine Learning taught by Jason Eshraghian, 

I was tasked with building a Leaky Integrate and Fire Neuron (LIFN) to explore how the computational principles of the brain can be harnessed to build ultra-efficient machine learning models in both software and hardware. 
When implemented in Spiking Neural Networks (SNNs), LIFNs can be 95% to over 99% more energy-efficient (or 20x to 100x lower energy consumption) than traditional artificial neural networks (ANNs), using ReLU activations. This efficiency arises because LIFNs are event-driven, meaning they only consume power when firing a spike, rather than performing high-precision floating-point multiplications for every neuron in every layer at every time step.

This particular LIFN's verilog HDL was built with a high level synthesis (HLS) tool I previously studied in a different class, PyMTL3 (https://pymtl.github.io/). 

This project was fabricated on the **TinyTapeout 5** shuttle using the **Skywater130 PDK**.

- **3-D representation of chip: https://gds-viewer.tinytapeout.com/?model=https%3A%2F%2Fshuttle-assets.tinytapeout.com%2Ftt05%2Ftt_um_hls_lfi%2Ftt_um_hls_lfi.oas&pdk=sky130A**

- Chip page: https://tinytapeout.com/chips/tt05/tt_um_hls_lfi