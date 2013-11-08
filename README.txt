COPYRIGHT & DISCLAIMER
----------------------

Copyright (C) 2013 MakeStuff (http://makestuff.eu)

This documentation describes Open Hardware and is licensed under the CERN Open
Hardware Licence v1.2. You may redistribute and modify this documentation under
the terms of the CERN OHL v1.2 (http://ohwr.org/cernohl). This documentation is
distributed WITHOUT ANY EXPRESS OR IMPLIED WARRANTY, INCLUDING OF
MERCHANTABILITY, SATISFACTORY QUALITY AND FITNESS FOR A PARTICULAR PURPOSE.
Please see the CERN OHL v1.2 for applicable conditions.


MAKESTUFF LX9 BOARD v1.1
------------------------

Features:
   * 80mm x 80mm, 4-layer PCB (KiCad-designed).
   * CERN OHL v1.1 licence.
   * Xilinx Spartan-6 LX9 FPGA[2].
   * Uses FPGALink[3] for programming & host communication.
   * Cypress FX2LP Hi-Speed USB interface (~45 MByte/s: see [4]).
   * 46 FPGA I/Os on top edge-connector, well-grounded.
   * SPI-bus and 8 FX2LP I/Os on bottom edge-connector.
   * 16 MBytes of SDRAM (see [5]).
   * SD-card slot.
   * 4 Mbit config flash (~40% free for application data).
   * Flexible power options.

   * A Xilinx Spartan-6 LX9 FPGA
   * A Cypress FX2LP Hi-Speed USB microcontroller
   * A 16MiB SDRAM, 16 bits wide
   * An SD-card slot
   * A well-grounded 80-way 2mm-pitch edge-connector with 47 FPGA I/Os
   * A second 2mm edge-connector with the FX2LP's port D and the SD card pins
   * A 1Mib EEPROM for the FX2LP firmware, FPGA design & initialisation data
   * FPGALink-compatibility

It is intended to be small enough and cheap enough to be used as a building-
block for larger FPGA-based projects, and to be solderable at home with the bare
minimum of tools (i.e no reflow oven, just a decent soldering iron). The
component cost for a small (e.g 10-off) run comes to about $40 for each board,
including the PCB.

The design files are in KiCad format (http://www.kicad-pcb.org). I used this:

http://iut-tice.ujf-grenoble.fr/cao/kicad-2012-01-19-BZR3256-stable-UBUNTU_10.10_full_with_components_doc.tgz

...running on x86_64 Ubuntu 12.04.
