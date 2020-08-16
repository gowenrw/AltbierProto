# AltbierProto

KiCad EDA project folder for the Altbier Proto PCB

## File Structure

This is the file structure of this repository

* ./<filename>.pro - project file. Holds parameters that apply to the entire project (e.g. schematic, PCB layout, etc.).
* ./<filename>.sch - schematic file.
* ./<filename>.kicad_pcb - the PCB New layout file.
* ./<filename>.net - netlist in "Pcbnew" format
* ./<filename>.bak - backup of schematic file.
* ./<filename>.kicad_pcb-bak - backup of the new PCB layout file.
* ./<filename>-cache.lib - a local cache copy of all the symbols used in the schematic
* ./fp-lib-table - Footprint library list
* ./sym-lib-table - Schematic library list
* [./3d_models/](/eda/prod/3d_models/) - This directory contains footprint 3d model files
* [./gerber/](/eda/prod/gerber/) - This directory contains gerber formatted files for manufacturing
* [./lib_fp/](/eda/prod/lib_fp/) - This directory contains footprint module directories
* [./lib_sh/](/eda/prod/lib_sh/) - This directory contains schematic library files
* [./snapshots/](/eda/prod/snapshots/) - This directory contains prints of schematic / cad files and images of preview / final product

## PCB Notes

Solderable breadboard with some SMD component pads.

* The THT holes are at 2.54mm pitch
* The TSSOP/SSOP-20 SMD for CH552T and similar chips also supports the 16, 14 and 8 pin 4.4mm wide varieties of this chip package type
* The SOIC/SOP-16 SMD for CH552G and similar chips also supports the 14 and 8 pin 3.9mm wide varieties of this chip package type
* The USB SMD connector is designed to fit a USB Micro package by Jing Ext which is a Micro B Female USB 2 5 SMD and is available via [LCSC.COM](https://lcsc.com/product-detail/USB-Connectors_Jing-Extension-of-the-Electronic-Co-C77238_C77238.html)
* There are six each of the SMD package sizes 1206, 0805, and 0603 which are all tied to THT holes for easy interconnections
