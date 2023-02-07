# Lab 7 - Sensor Changes - February 07, 2023

Connecting the joystick to arduino, responding to changes in sensor data, writing with specific instead of constant serial data

## Prep

Some notes from reviewing the lab doc:

* **Joystick:** Potentiometer for both X and Y axis, switch for pushbutton.
* **Joystick** to **Arduino**
* GND > GND
* +5V > 5V
* VRx > A0
* VRy > A1
* SW  > D3

## Process

### Excercise 1: Reading potentiometer and switch data from the joystick

* I connected the joystick to the arduino, copied the code from the lab doc, built, and uploaded it.

![Photo of joystick connected to arduino](images/l7e1Wiring.png)

* The serial monitor started printing an endless barage of data values

![Screenshot of Serial monitor displaying an erroneous wall of data from the joystick](images/l7e1Serial1.png)

* Upon further inspection, I realised that I had mistakenly omitted "ln" the last "Serial.print" function, creating that error. With that fixed, the serial monitor started displaying accurate data.

![Screenshot of properly functioning serial monitor](images/l7e1Serial2.png)

* It became obvious to me that the origin is not in the center "resting" state of the joystick, but actually in the upper left corner, as with p5js...

* With that said, I can make the assumption that the X axis actually accounts for more range of motion than the y axis.

* **Pullup Resistor:** Alleviates "floating" pins by "pulling" the pin to HIGH when the switch isn't activated
  
* The arduino contains an on-board pullup resistor, activated by INPUT_PULLUP

* Next, I copied the remaining code to read the switch.

![Screenshot of properly functioning serial monitor, now displaying switch value](images/l7e1Serial3.png)

### Excersise 2: Responding to Changes in the State of a Sensor

## Conclusion
