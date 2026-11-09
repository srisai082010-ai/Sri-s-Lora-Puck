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
this is some of the porject photos:
<img width="370" height="374" alt="Screenshot 2026-11-08 194500" src="https://github.com/user-attachments/assets/b507e28f-c36c-4b33-aeda-5cb03a30a6b9" />
<img width="1007" height="573" alt="Screenshot 2026-11-08 183346" src="https://github.com/user-attachments/assets/ee830ced-ccd4-4cf9-85d7-6f97a4bbde50" />
<img width="1173" height="799" alt="Screenshot 2026-11-08 133103" src="https://github.com/user-attachments/assets/c0d94474-d2bd-4b38-9957-cfe840cc54e4" />

