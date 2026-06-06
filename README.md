# BIT90/26
An attempted recreation of the BIT90 computer released by Bit Corporation (普澤有限公司) in 1983 that is about [US$90,000 (AU$125,000) cheaper than a used one](https://web.archive.org/web/20260206154213/https://www.ebay.com/itm/127471879150):<br>
- Z80 CPU
- TMS9929A VDP
- 2KB RAM (one TC5517/4016 SRAM) expandable to 32KB (expansion cartridge)
- 16KB VRAM (eight 4116 DRAM)
- 24KB ROM (two 2364 + one 2764 or a variation) containing BASIC & Colecovision firmware (?)
- RF & composite video output
- two joystick ports
- Colecovision cartridge/tape compatible (2x15 pin)
- combination audio/video/tape port (DE9)
- expansion edge connector (2x30 pin)
- 5-pin DIN for power (±5V & +12V)

![BIT90 original](https://github.com/b3rendsh/bit90/blob/main/images/BIT90.jpg)

Heavily relying on all the excellent information shared by [b3rendsh](https://github.com/b3rendsh) in their [BIT90 repository](https://github.com/b3rendsh/bit90).<br>

## [Part 1](/KiCad/BIT90_Original/) - Completed (enough)
The initial aim of the project is to recreate the original schematics in KiCad:<br>
- Sheet 6-1 (Processor): ✅ completed
- Sheet 6-2 (Video Control): ✅ completed
- Sheet 6-3 (Joystick, Audio, Tape): ✅ completed
- Sheet 6-4 (Keyboard): ✅ completed
- Sheet 6-5 (PAL Video Encoder): ❌ lost interest
- Sheet 6-6 (Expansion): ✅ completed
- Sheet 7-5 (PAL Video Encoder/32K): 🤔 pending
- 32K DRAM (4416x4): 🤔 pending

The Video Encoder schematic isn't really relevant to my proposed re-design so haven't bothered completing them.<br>

Sheet 7-5 and the 32KB DRAM sheets appear to be for an updated system with 32KB of RAM?  This would be the ultimate aim, but let's see if we can get the initial 8KB system working.<br>

## Part 2 - Ongoing
The second part will be to try to create a modern replica as a single board computer.<br>

Ideally:
- integrated keyboard
- upgraded 8KB of RAM
- replace VDP9929A & 16KB DRAM with a [Pico9918](https://github.com/visrealm/pico9918)
- HDMI video output (thanks to the Pico9918)
- replace tri-voltage ±5VDC & 12VDC power requirement with a single 5VDC via USB or 2.1mm socket

The main hurdle would be sourcing the SN76489AN sound generator but I don't think this is ... currently (June 2026) ... too difficult. If you are wary of Chinese sellers, a reliable source of genuine parts is [Unicorn Electronics](https://unicornelectronics.com/IC/GENERATORS.html) in the US.  Grab yourself some EPROMs or exotic CPUs whilst you're there.<br>

## Keyboard
Recreation of the original keyboard layout.<br>
Designed with [Keyboard Layout Editor](https://www.keyboard-layout-editor.com/) which generates a JOSN file that can be used to generate a template for the key switches with [Plate & Case Builder](http://builder.swillkb.com).<br>

![Keyboard layout](/Keyboard/bit90-keyboard.png)

## ROMs
The original ROMs have been dumped and can be found [here](https://forums.atariage.com/topic/296435-bit-90-computer-roms-finally-dumped/).<br>

## BBC Basic
You can now also use a version of BBC Basic on the BIT90 thanks to [b3rendsh's](https://github.com/b3rendsh) work developing [BBX80](https://github.com/b3rendsh/bbx80).<br>

## Status
- 3/JUN/2026: Working on [Part 1](/KiCad/BIT90_Original/)
- 4/JUN/2026: Keyboard layout re-created & template generated
- 5/JUN/2026: Initial redesign [(schematic)](/KiCad/BIT90_26/) completed, error checking/fixing to follow
- 6/JUN/2026: PCB layout started
