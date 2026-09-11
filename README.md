# 5V Regulated BC548 Driver Test Board

A through-hole test/practice board combining a 5V linear regulator stage with a dual-BC548 transistor driver stage.

## Hardware

### Power Input / Main sheet
- **J1** - 2-pin XT30 connector (power input)
- **D3 - 1N4001** - reverse-polarity protection diode
- **J7** - 10-pin JST-PH connector (I/O header)

### Regulator Section
- **U1 - LM7805 (TO-220)** - 5V linear voltage regulator
- **D2 - 1N4148** - protection diode
- **C1, C3** - 470nF filter caps
- **C2** - 10uF filter cap
- **C4** - 1000uF bulk filter cap
- **TP3** - +5V test point

### Display and Transistor
- **Q1, Q2 - BC548** (TO-92) - NPN driver transistors
- **R1, R4** - 10k bias resistors
- **R2** - 22k resistor
- **R13, R14** - 470Ω output resistors
- **TP8** - test point

## Repo structure
- `5V-Regulated-BC548-Driver-Test-Board.kicad_sch` (main) / `Regulator Section.kicad_sch` / `display and transistor.kicad_sch` - schematics
- `.kicad_pcb` / `.kicad_pro` / `.kicad_prl` - KiCad project files
- `Bill of materials/` - BOM (CSV)
- `Component placement/` - pick-and-place position file
- `Garber file/` - manufacturing gerbers + PTH/NPTH drill files + job file

**Scope:** hardware/PCB design only, through-hole build.
