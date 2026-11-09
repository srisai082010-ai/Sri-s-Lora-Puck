# Sri's LoRa Puck

A custom four-layer LoRa PCB designed in **KiCad 10**, following the [Hack Club Blueprint LoRa Puck guide](https://blueprint.hackclub.com/starter-projects/lora).

> **Work in progress:** Schematic design and initial PCB component placement have been prepared. Routing, design-rule checking, manufacturing, and hardware testing are not complete.

## About the project

I'm building a LoRa development board to learn schematic capture, PCB layout, power management, microcontrollers, and radio-frequency design. The board brings together a microcontroller, radio, USB-C connectivity, memory, and an RF antenna path.

## Main hardware

| Component | Purpose |
| --- | --- |
| RP2040 (U2) | Main microcontroller |
| SX1261IMLTRT (U1, currently labeled) | LoRa radio |
| W25Q128JVS (U4) | Flash memory |
| USB-C receptacle (J1) | USB connection and power input |
| AP2112K-3.3 (U5) | 3.3 V power regulation |
| PE4259 (U3) | RF switch |
| 0900FM15K0039 (FL1, currently labeled) | RF front-end component |
| 32 MHz crystal (Y1) | Radio clock |
| BOOTSEL and RESET buttons | Board control |

**Verification needed:** My current schematic lists SX1261IMLTRT and 0900FM15K0039, while the Blueprint guide references an SX1262-based design and a differently numbered RF component. I need to confirm exact part numbers, pinouts, footprints, and radio compatibility before fabrication. The Y2 crystal value also needs verification.

## Design progress

- [x] Create KiCad schematic
- [x] Assign footprints
- [x] Create an initial PCB component placement
- [ ] Verify component values and footprint selections
- [ ] Complete routing and copper zones
- [ ] Run and pass KiCad ERC and DRC
- [ ] Review manufacturing files and bill of materials
- [ ] Assemble and test the physical board

## PCB design goals

- Four-layer PCB stack-up
- Keep crystal and decoupling components close to their associated ICs
- Keep the radio-frequency routing short, with a verified controlled-impedance design
- Make USB-C power and grounding reliable
- Check antenna placement and clearances before manufacturing

## Opening the project

Install **KiCad 10**, then open the KiCad project, schematic, and PCB files after they have been uploaded to this repository. Custom symbols and footprints must also be included where required.

## Credits

Based on the [Hack Club Blueprint LoRa Puck starter project](https://blueprint.hackclub.com/starter-projects/lora). 

See [Hardware Notes](HARDWARE_NOTES.md) for design checks and remaining work.
