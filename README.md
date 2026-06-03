# BIT90/26
An attempted recreation of the BIT90 computer released by Bit Corporation (普澤有限公司) in 1983 that is about [US$90,000 (AU$125,000) cheaper than a used one](https://web.archive.org/web/20260206154213/https://www.ebay.com/itm/127471879150):<br>
- Z80 CPU
- TMS9929A VDP
- 2KB RAM (one TC5517/4016 SRAM)
- 16KB VRAM (eight 4116 DRAM)
- 16KB ROM (two 2732 + one 2764?)
- RF & composite video output
- two joystick ports
- Colecovision cartridge/tape compatible (2x15 pin)
- combination audio/video/tape port (DE9)
- expansion edge connector (2x30 pin)
- 5-pin DIN for power (±5V & +12V)

![BIT90 original](https://github.com/b3rendsh/bit90/blob/main/images/BIT90.jpg)

Heavily relying on all the excellent information shared by [b3rendsh](https://github.com/b3rendsh) in their [BIT90 repository](https://github.com/b3rendsh/bit90).<br>

## [Part 1](/KiCad/BIT90_Original/) - Work In Progress
The initial aim of the project is to recreate the original schematics in KiCad:<br>
- Sheet 6-1 (Processor): completed
- Sheet 6-2 (Video Control): completed
- Sheet 6-3 (Joystick, Audio, Tape): completed
- Sheet 6-4 (Keyboard): completed
- Sheet 6-5 (PAL Video Encoder): pending
- Sheet 6-6 (Expansion): completed
- Sheet 7-5 (PAL Video Encoder/32K): pending
- 32K DRAM (4416x4): pending

Sheet 7-5 and the 32KB DRAM sheets appear to be for an updated system with 32KB of RAM?<br>

## Part 2
The second part will be to try to create a modern replica as a single board computer with integrated keyboard.<br>

This will include changes like replacing the original DRAM with modern SRAM which, in turn, should mean we can get rid of the original tri-voltage power supply requirement with a single 5V supply.<br>

## ROMs
The original ROMs have been dumped and can be found [here](https://forums.atariage.com/topic/296435-bit-90-computer-roms-finally-dumped/).<br>

## BBC Basic
You can now also use a version of BBC Basic on the BIT90 thanks to [b3rendsh's](https://github.com/b3rendsh) work developing [BBX80](https://github.com/b3rendsh/bbx80).<br>

## Status
- 3/JUN/2026: Working on [Part 1](/KiCad/BIT90_Original/).<br>
