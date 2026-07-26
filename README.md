# Dual Digital Dice Circuit

A hardware-based dual digital dice simulator designed and built as an EEE2204 course project at Bahçeşehir University.

The circuit generates two independent pseudo-random values and displays them on separate seven-segment displays. It is implemented entirely with standard digital and analog ICs; no microcontroller or programmable device is used.

## Design

Each die has an independent signal chain:

1. A 555 timer generates the clock signal.
2. A CD4017 decade counter advances through the dice values.
3. A 7447 BCD-to-seven-segment decoder drives the display.
4. A push-button control simulates rolling both dice.

Using separate clock sources allows the two dice to change asynchronously and reduces the chance of identical output patterns.

## Main components

- 2 x NE555 timer IC
- 2 x CD4017 decade counter
- 2 x 7447 BCD-to-seven-segment decoder
- 2 x seven-segment display
- Push button, resistors, capacitors, LEDs, and supporting components

## Repository contents

- [`docs/project-report.pdf`](docs/project-report.pdf): Design methodology, prototype development, testing, and photographs
- [`docs/bill-of-materials.pdf`](docs/bill-of-materials.pdf): Updated component list

## Project status

The physical prototype was completed and tested. The original editable schematic/simulation files were not present in the archived project folder, so this repository currently preserves the verified documentation only.

## Authors

Developed by Andaç Ünal and Ayşe Ece Nail.

