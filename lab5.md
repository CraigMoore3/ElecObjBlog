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

! [Breadboard layout for LCD Display](images/lab5Breadboard.png)

* Next, I copied the code from the doccument and read through the notes and key to understand what each line's function was.

* Having accessed the code, I uploaded it to the arduino and had success.

! [LCD Display: Hello World!](images/lab5LCD1.png)

* To finish the lab, I experimented with displaying different strings of text on the LCD.

! [LCD Display: Lab 5 Complete](images/lab5LCD2.png)

## Conclusion

* In the end, this lab was pretty easy with the help of the instructions. Although I think that I'm lacking some of the foundational knowledge of the layout of the LCD Display, I think that this lab taught me enough to display text on and LCD in future projects.
