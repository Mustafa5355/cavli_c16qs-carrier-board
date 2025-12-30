# cavli_c16qs-carrier-board

This repository contains the complete hardware design for a 2-layer carrier board for the Cavli C16QS LTE Cat-1 bis module. The board provides regulated power, SIM card interface, RF antenna connection via u.FL, level-shifted UART communication to a 3.3 V host, and control/status signals.

The design is implemented in KiCad and follows Cavli's hardware guidelines for power integrity, RF layout, and SIM protection. It is intended as a reference carrier for evaluation, prototyping, and integration of the C16QS module into embedded systems.

Features:
- 5 V input with synchronous buck regulation to module VBAT
- Nano-SIM socket with ESD protection and signal conditioning
- u.FL connector for external LTE antenna
- Bidirectional UART level shifting between 1.8 V and 3.3 V domains
- Hardware power key, reset, and network status indication
- 2-layer, low-cost PCB optimized for EMI and signal integrity

The repository includes schematic, PCB layout, fabrication outputs, BOM, and design documentation.

## Footprint Note

The C16QS footprint included in this repository was created manually by the author using the published mechanical drawings and pin mapping of the C16QS module. It is designed to be reusable across projects and is suitable for prototyping and evaluation.

This footprint is not an official manufacturer CAD file. Users should verify alignment and pin mapping against the latest Cavli documentation before fabrication.
