# BIT90/26
An attempted recreation of the HIT90 computer from 1983:<br>
- Z80 CPU
- TMS 9929A VDP
- 16KB RAM (eight 4116 DRAM)
- 2KB VRAM (one 4016 SRAM)
- 16KB ROM (two 2732 + one 2764?)
- two joystick ports
- Colecovision cartridge/tape compatible
- combination audio/video/tape port (DE9)
- expansion edge connector
- 5-pin DIN for power (±5V & +12V)

Heavily relying on all the excellent information shared by [b3rendsh](https://github.com/b3rendsh) in their [BIT90 repository](https://github.com/b3rendsh/bit90).<br>

## [Part 1](/KiCad/BIT90_Original/) - Work In Progress
The initial aim of the project is to recreate the original schematics in KiCad.<br>

## Part 2
The second part will be to try to create a modern replica as a single board computer with integrated keyboard.<br>

This will include changes like replacing the original DRAM with modern SRAM which, in turn, should mean we can get rid of the original tri-voltage power supply requirement with a single 5V supply.<br>

## Status
- 3/JUN/2026: Working on [Part 1](/KiCad/BIT90_Original/).<br>
