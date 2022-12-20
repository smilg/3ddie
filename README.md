# 3ddie
3D Digital Interface, EPIC!

## Project Structure
[3ddie/](3ddie/): contains the Kicad (6.x) project for 3ddie. This includes the schematic, board layout, [BOM](3ddie/3ddie-bom-cleaned.csv), symbols, and footprints.

[mcad/](mcad/): contains SOLIDWORKS assembly files for 3ddie and the beginnings of a case.

[firmware/](firmware/): contains firmware for 3ddie. Currently, this only includes the start of the I²C to USB bridge firmware for the RP2040 to allow connection between the MGC3130 and Microchip's Aurea software. The submodules in that folder are projects that we are basing this off of.

[silkscreen_images/](silkscreen_images/): contains the image files for the silkscreen art on the PCB. These were converted to footprints using Kicad:s built-in tool.
