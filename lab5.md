# Lab 5 - LCD Display - January 31, 2023

Wiring and Controlling LCD Display with Arduino UNO

## Prep

* I started the lab, as always, by reading through the lab doccument a few times, familiarizing myself with the process, materials, and concepts that we will be covering.

### LCD Pin Layout

* **VSS:** Ground
* **VDD:** +5V Power supply
* **VO:** Adjusts Contrast
* **RS:** Register Select: Location in memory where data is written
* **R/W:** Read/Write Selection
* **E:** Enabling, executing instructions
* **D0-D7:** Reads/Writes Data
* **A and K:** Backlight Control

## Process

* I started by working from the wiring diagram to create my breadboard circut. The Diagram itself confused me because the pins on the LCD were not labled, but the connection schematic resolved that trouble. It took some focus, but it eventually came together

Image

* Next, I started copying the code from the doccument.
