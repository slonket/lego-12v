# Lego 12V

### An assortment of projects to supplement the Lego 12V "Gray" era trains.

## Project Structure

This is the high-level directory for projects within this repository. All projects follow the same general file structure, though some hierarchical items may be missing if the project does not require them (e.g. `/firmware/` for a project without an MCU):
- `/hardware/` - PCBA project.
    - `/panel/` - panelized PCBA project for manufacturing.
    - `/production_files/` - production files for the PCBA project (including BOM and POS files).
- `/firmware/` - embedded firmware for MCU(s) contained within PCBA project.
- `/mechanical/` - 3D models (`.step`) for the physical item(s).
    - `/outlines/` - 2D profiles (`.dxf`) related to PCB design, etched parts, etc.

### Miscellaneous Items

Some items do not pertain to a higher level project and can be found within the `/_misc/` directory. These are individually documented with a brief description in `/_misc/README.md`.

## PCBA

### PCBA Production

The PCBA projects are designed with production using JLCPCB in mind. As such, the exported gerbers, placement, and BOM files are all formatted for JLCPCB and their parts library. Detailed instructions for ordering parts can be found within each project.

### KiCAD Libraries

All PCBA projects within this repository use the Slonket KiCAD libraries. If you wish to modify a PCBA project, you will need to download the [Slonket Footprints](https://github.com/slonket/slonket-footprints) repository and add the contained libraries as "Global" within KiCAD. You do not need to use KiCAD when ordering items within this repository - as detailed above, each project already contains the necessary production files for ordering.