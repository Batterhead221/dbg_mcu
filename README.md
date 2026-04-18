
# dbg_mcu (STM32_MICROCONTROLLER)

# V1.1

![dbg_mcu](/outputs/img/repo_img/hero.png)

-USB-C (USB 2.0) STM32F072CBT6-based programmer/debug adapter board.

- USB-C powered + USB 2.0 device interface
- Target programming/debug via **SWD**
- Dedicated reset control and debug access points
- On-board power section (labeled **POWER**) with switching and protection components

## Hardware overview
- MCU: **STM32F072CBT6**
- USB: **USB-C 2.0** (device/UFP configuration)
- Debug: **SWDIO / SWCLK / NRST / GND**
- Board: **DEBUGGER_V1.0**

## Connectors & headers
- **USB-C**: primary power + USB data connection
- **J2 (DEBUG header)**: main target interface header (SWD + reset + power reference)
- **J1 / J3 / S1 / S2**: board configuration/jumper/select features (see silkscreen)

## Test points (silkscreen labels)
- **TP2_3V3**: 3.3V rail test point
- **TP3_GND**: ground reference test point
- **TP4_NRST**: target reset test point
- **TP5_SWDIO**: SWD data test point
- **TP6_SWCLK**: SWD clock test point

## On-board power (POWER block)
Located on the left side of the board (near **SW1** and components marked U3/U4).
- Input comes from USB-C 5V
- Generates and distributes rails used by the MCU/debug interface
- Protection/fusing present (F1)

## Buttons / switches
- **RESET area (SW2)**: reset functionality (see silkscreen)
- **SW1 (POWER area)**: power-related switching (see silkscreen)

## PROGRAM/DEBUG HEADER
J2 pinout reference:
- Pin 1: +3V3
- Pin 2: SWDIO
- Pin 3: GND
- Pin 4: SWCLK
- Pin 5: GND
- Pin 10: NRST

DESIGNED & ENGINEERED BY BRANDON SHELLY