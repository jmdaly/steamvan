# SteamVan PCB

The SteamVan was developed as a MiniVan-compatible PCB based on an STM32MCU. It
does not support hot swap sockets, and it is designed such that the switches
are oriented such that the LEDs are South-facing.

## Overview

The SteamVan aims to meet the following design goals:

* Switches oriented such that the LEDs are South-facing, for
  compatibility with Cherry profile keycaps.

* USB Type-C support in both A to C and C to C configurations.

* QMK support.

* ESD protection circuitry, including data line protection and a
  polyfuse on the VCC line.

* Support for per-switch LED backlighting.

* Fits in MiniVan keyboard cases (tested with R3 MiniVan case only)

* RGB LED underglow support. (Note that, at present, RGB underglow support is
  not merged into QMK master for STM32 PCBs.)

## Supported Layouts

The SteamVan supports the same layout options as the MiniVan.

## Obtaining the Files

This repository contains several submodules, which in turn contain
KiCad libraries used in the PCB design. In order to clone the SteamVan
repository, and all of the library submodules, the following command
must be issued,

```
git clone --recursive https://github.com/jmdaly/steamvan.git
```

## Acknowledgements

This project would not have been possible without all of the awesome work put
in by Evan Sailer of thevankeyboards.com. I own an R3 MiniVan and I love it. I
really like PCBs that have South-facing LEDs, USB-C connectors, and STM32
microcontrollers. As a result, I took on this project so that I could continue
to use the MiniVan layout, as well as my MiniVan case and keycaps, but have
some of the features that are important to me in a keyboard. I hope this work
is useful to other people.

There is an active keyboard design community on the MechKeys discord. The
users there have been very helpful, and I've learned a significant
amount about PCB design from them.
