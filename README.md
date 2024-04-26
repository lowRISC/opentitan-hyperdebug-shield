# OpenTitan

![OpenTitan logo](https://docs.opentitan.org/doc/opentitan-logo.png)

## About the project

[OpenTitan](https://opentitan.org) is an open source silicon Root of Trust
(RoT) project.  OpenTitan will make the silicon RoT design and implementation
more transparent, trustworthy, and secure for enterprises, platform providers,
and chip manufacturers.  OpenTitan is administered by [lowRISC
CIC](https://www.lowrisc.org) as a collaborative project to produce high
quality, open IP for instantiation as a full-featured product. See the
[OpenTitan site](https://opentitan.org/) and [OpenTitan
docs](https://opentitan.org/book) for more information about the project.

## About this repository

This repository contains the manufacturing files for the OpenTitan Hyperdebug Shield development platform, codenamed 'TEACUP' 
created as part of the OpenTitan project. It is structured as a monolithic repository, or "monorepo",
where all components live in one repository. It exists to enable collaboration
across partners participating in the OpenTitan project.

### What is the OpenTitan Hyperdebug Shield?

![hyp_ot](/images/hyp_ot.png)

The OpenTitan Hyperdebug Shield, codenamed TEACUP, is a development board which connects to the STM32F552 Nucleo, (ST Part Number: [NUCLEO-L552ZE-Q
](https://www.st.com/en/evaluation-tools/nucleo-l552ze-q.html). This development board allows for developing and provisiong of Nuvoton's
implementation of OpenTitan, the NPCR100T.

The OpenTitan Hyperdebug Shield contains:
- 1x BOYD Corp. 718-SW08105-508-B1 9x9 0.5mm BGA socket (Socket Optional)
- 1x DEDIPROG TECHNOLOGY SOK-SPI-WSON68-L WSON68 flash socket (Socket Optional)
- 1x USBC, USB 2.0 connector (without PD/BC1.2)
- 2x MICROCHIP TECHNOLOGY INC. PAC1954T-E/4MX
- 1x ISSI IS31FL3205-QFLS4-TR LED Driver
- 4x RGB LEDs
- 4x Zio connectors
- 1x JTAG connector

![hyp_ot_bd](/drawings/hyp_ot_blockdiagram.png)

Note: 
Sockets are provided for both the NPCR100T as well as the WSON8 flash. 
Both sockets are optional, giving the ability to have the NPCR100T as well as the WSON68 flash soldered down instead.

## Repository Directory

The project contains manufacturing documentation of the OpenTitan Hyperdebug Shield. 
For detailed documentation of the software and tooling, please see [docs.opentitan.org](https://docs.opentitan.org/).

### Projects top-level directory

    .
    ├── bom                     # Bill Of Materials
	├── drawings                # Schematics and Assembly Drawings
	├── gerbers                 # Gerbers, Drill Drawings and other output files for PCB Fab and Assembly
    ├── images                  # Images used on this repository
    └── README.md				# This file

## Licensing

Unless otherwise noted, everything in this repository is covered by the Apache
License, Version 2.0 (see [LICENSE](https://github.com/lowRISC/opentitan-hyperdebug-shield/LICENSE) for full text).