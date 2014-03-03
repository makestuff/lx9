COPYRIGHT & DISCLAIMER
----------------------

Copyright (C) 2014 MakeStuff (http://makestuff.eu)

This documentation describes Open Hardware and is licensed under the CERN Open
Hardware Licence v1.2. You may redistribute and modify this documentation under
the terms of the CERN OHL v1.2 (http://ohwr.org/cernohl). This documentation is
distributed WITHOUT ANY EXPRESS OR IMPLIED WARRANTY, INCLUDING OF
MERCHANTABILITY, SATISFACTORY QUALITY AND FITNESS FOR A PARTICULAR PURPOSE.
Please see the CERN OHL v1.2 for applicable conditions.


MAKESTUFF LX9 BOARD REV3
------------------------

Features:
   * 80mm x 80mm, 4-layer PCB (KiCad format).
   * Xilinx Spartan-6 LX9 FPGA[1].
   * Uses FPGALink[2] for programming & host communication.
   * Cypress FX2LP Hi-Speed USB interface (~45 MByte/s).
   * 46 FPGA I/Os on top edge-connector, well-grounded.
   * SPI-bus and 8 FX2LP I/Os on bottom edge-connector.
   * 16 MBytes of SDRAM.
   * SD-card slot.
   * 4 Mbit config flash (~40% free for application data).
   * Flexible power options.

It is intended to be small enough and cheap enough to be used as a building-
block for larger FPGA-based projects, and to be solderable at home with the bare
minimum of tools (i.e no reflow oven, just a decent soldering iron). The
component cost for a small (e.g 10-off) run comes to about $40 for each board,
including the PCB.

The design files are in KiCad format (http://www.kicad-pcb.org). I used this:

http://iut-tice.ujf-grenoble.fr/cao/old_versions/kicad-2012-01-19-BZR3256-stable-UBUNTU_10.10_full_with_components_doc.tgz

...running on x86_64 Ubuntu 12.04.

[1]http://www.xilinx.com/products/silicon-devices/fpga/spartan-6/lx.htm
[2]http://www.makestuff.eu/wordpress/software/fpgalink
