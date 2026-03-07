+++
title = "TinyTapeout 6 — HSC TDCs with various delay lines"
date = "2024-04-20T00:00:00Z"
draft = false
tags = ["tinytapeout", "asic", "open-source-silicon"]
summary = "TinyTapeout 6 shuttle tapeout: full add, mux, and buffer TDC variants."
thumbnail = "https://phillipmmarlowe.github.io/professionalpm/images/tinytapeout6chip.png"
+++

## Overview

During the beginning of my time at the Hardware Systems Collective (my research group), I assisted Tyler Sheaves in contruction of various delay line elements within a Time-to-Digital Converter (TDC) to be used to measure the effects of BTI on MOSFET trasistors.
A TDC is a circuit that measures very small time differences, on the scale of nano to picoseconds, by turning them into a digital value. In these chips linked below, the TDC launches a rising or falling signal edge into a delay line made of many small logic elements, then captures the state of that line with registers at a specific clock instant. The point the transition has reached along the delay line tells you how much time has passed between launch and capture, so time is encoded as a bit position which is then outputted as a Hamming Weight distance. The propagation speed through the delay line varies slightly with supply-voltage fluctuations in the FPGA’s power distribution network, a TDC can also serve as a sensitive sensor. Changes in power consumption from nearby logic affect how far the transition travels during the sampling window, potentially revealing information about co-located activity.
I constructed and, buf, and mux delay lines to be taped out in the TinyTapeout 6 Shuttle using the Skywater130 PDK. Size and spacing constraints were necessary in achieving the desired uniform delay line. A synopsis design constrait (.sdc) file was used to accomplish this.


This project was fabricated on the **TinyTapeout 6** shuttle using the **Skywater130 PDK**.

- **3-D representation of full add carry chain delay line chip: https://gds-viewer.tinytapeout.com/?model=https%3A%2F%2Fshuttle-assets.tinytapeout.com%2Ftt06%2Ftt_um_hsc_tdc%2Ftt_um_hsc_tdc.oas&pdk=sky130A**

Chip pages:
- https://tinytapeout.com/chips/tt06/tt_um_hsc_tdc
- https://tinytapeout.com/chips/tt06/tt_um_hsc_tdc_mux
- https://tinytapeout.com/chips/tt06/tt_um_hsc_tdc_buf