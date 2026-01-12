## AstraDev
- AstraDev is a custom-designed development board created for embedded systems learning, prototyping, and real-world hardware design experience. The project follows a complete professional workflow—from schematic design to PCB layout, 3D verification, and manufacturing preparation.

# Project Overview
- AstraDev was designed to demonstrate a full PCB development lifecycle using industry-standard practices. The board design emphasizes clean schematics, organized PCB routing, proper grounding, and manufacturing readiness. All files have been verified and prepared for fabrication and assembly through JLCPCB.

# Schematic Design
- The schematic was designed using KiCad Schematic Editor
- All functional blocks were clearly separated:
Power supply and regulation
Microcontroller and clock circuitry
USB interface
Programming/debug interface
GPIO and peripheral connections
CUSTOM DEVBOARD guide-recommended components such as decoupling capacitors, pull-up/down resistors, and protection elements were included
Net labels and reference designators were standardized for clarity
Electrical Rule Check (ERC) was performed to ensure there were no schematic errors
The schematic was finalized and locked before PCB layout

# PCB Layout and Wiring

- PCB layout was completed using KiCad PCB Editor
- A 2-layer PCB was used:
Top layer (F.Cu) for signal routing
Bottom layer (B.Cu) primarily for ground plane and routing
Components were placed using functional grouping to reduce track length and noise
Power tracks were routed first, followed by critical signals and GPIO lines
Track widths were selected based on signal type:
GPIO and signal lines: minimum safe width
Power lines: wider tracks
A GND copper pour was added on both layers for proper grounding
Thermal reliefs and clearances were adjusted to ensure good solderability
Via stitching was used where necessary to improve ground connectivity
Design Rule Check (DRC) was run and all errors were resolved before production

# 3D Viewer Verification

- KiCad’s 3D Viewer was used to visually inspect the PCB
Component orientation, alignment, and placement were verified
Mechanical fit of connectors (USB, headers) was checked
Potential assembly issues were identified early
This step ensured the PCB would be physically correct before manufacturing

-  Manufacturing File Preparation:
Gerber and drill files were generated from KiCad
files were verified using Gerber viewer tools
A Bill of Materials (BOM) was generated and modified to meet JLCPCB requirements
A Component Placement List (CPL / Pick-and-Place) file was generated from the PCB editor
BOM and CPL headers were renamed to match JLCPCB’s accepted format
Only top-side assembly files were included
All production files were organized into a single production folder and compressed into a ZIP archive

# JLCPCB Checking and PCBA Preparation

- The production ZIP was uploaded to JLCPCB
PCB Assembly (PCBA) option was enabled
ENIG surface finish was selected for reliable soldering and flat pads
BOM components were reviewed:
Missing or incorrect parts were manually reassigned
Basic parts were prioritized to reduce cost
Pin headers and non-essential components were excluded from assembly
Component orientation and placement were verified using JLCPCB’s online PCBA viewer
Final checks were completed before submission

# Production Status

- Schematic completed and verified

- PCB layout completed and DRC cleared

- 3D verification completed

- BOM and CPL prepared and validated

- Ready for JLCPCB fabrication and assembly

- Awaiting funding for order placement




# Designed and documented by ANBU
