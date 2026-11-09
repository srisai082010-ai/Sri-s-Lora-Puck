# Hardware Notes

## Status
This is an in-progress PCB design, not a tested or production-ready board. The uploaded design snapshot had 49 footprints and no completed copper trace routing.

## Design blocks
- RP2040 microcontroller and external flash
- SX126x radio section and clocks
- RF filter, switching, matching, and antenna
- USB-C, 3.3 V regulator, and board controls

## Before manufacturing
1. Confirm U1's radio part number: the schematic says **SX1261IMLTRT**, while the Hack Club guide uses SX1262.
2. Confirm the RF front-end FL1 part number and footprint: the current design says **0900FM15K0039**.
3. Correct and verify the Y2 crystal frequency and related components.
4. Check that the RP2040 core regulator output isn't shorted to the external 3.3 V rail.
5. Verify antenna clearances, RF trace impedance, and RF component placement against datasheets.
6. Add appropriate ground/power copper zones and verify grounding.
7. Complete the PCB routing, run ERC and DRC, inspect Gerber/drill files, and verify the BOM.
8. Test an assembled board before claiming successful RF operation.

Reference: https://blueprint.hackclub.com/starter-projects/lora
