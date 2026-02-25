{
   "date": "2023-10-19T00:40:04-07:00",
   "title": "Prototype PCB Milling"
   "tags": ["pcb", "milling", "prototyping"]
   "categories": ["projects"]
}

## Overview

I've milled 50+ 2‑layer prototype pcbs during my time at BELS for various classes such as Capstone Design, RF Hardware Design, and High Speed Digital Design.

## Process

- Import artwork files (top, bottom, board outline,) and isolate traces in circuitCAM gerber (min tolerance ~10 mils). 
- Ensure proper isolation and drill hole plating, to then export to Mill.
- Begin etching and drilling processes on Mill tool software (LPKF Boardmaster for me).
- Verify continuity and isolation quality.

## Example Finished PCB

{{< figure
  src="https://phillipmmarlowe.github.io/professionalpm/images/pcb_raw.png"
  alt="Finished milled PCB"
  title="Finished Board"
  caption="Finished milled 2‑layer PCB (unpopulated)."
  width="300"
  class="about-figure"
>}}
{{< figure
  src="https://phillipmmarlowe.github.io/professionalpm/images/pcb_gerber.png"
  alt="Board gerber view"
  title="Board in Gerber"
  caption="Gerber rendering showing top copper layer and board outline."
  width="300"
  class="about-figure"
>}}
{{< figure
  src="https://phillipmmarlowe.github.io/professionalpm/images/pcb_m60.png"
  alt="Mill software preview"
  title="Board in Mill Software"
  caption="Mill software preview (LPKF Boardmaster) showing milling and drill operations."
  width="300"
  class="about-figure"
>}}