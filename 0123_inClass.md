# January 23, 2023 - in class

## Arduino Notes

* Some pins have dedicated functions
* **0/1, Rx/Tx** - Recieve/transmit
* **~** - PWM (pulse width modulation)
* **13** - Onboard LED
  
* Hardware can add, subtract, mutliply
* Hardware cannot divide, instead, multiply by decimal

* Timer is always running, regardless of blocking
* Interuppts can be used to handle things like background blinking regardless of blocking

## Function Types

* void setup() { } *void functions do not return anything*
* some functions return (random)
* some need parameters {random(1,10)}

## Variable Scopes / Notes

* **Global** - Defined above setup, used throughout
* **Local** - Defined within function, used within braces

* **Const** - Variable that won't change
* **millis()** - Time since Arduino booted
* **=** - Sets Variable
* **==** - Compares variable

## Data Basics

* **Bit** - binary, 0 or 1
* **Byte** - 8 bits

* **Binary** - base 2, used by computers, low level programming language
* **Decimals** - base 10, used by humans

* 4-bit - nibble
* 8-bit - byte
* 16-bit - word
* 32-bit - long
* 64-bit - double long

## Data Types

* **Bool** - binary
* **Byte** - unsigned, (0, 255)
* **Char** - signed, (-127, 127)
* **Word** - (0, 65k)
* **Int** - signed
* **Float**

Plan on defaulting to bytes in most cases

## Things to check out

* Forraker Electronics
* Hobbytown USA
* Tamiya Motors
* Harbor Freight
* Ali Express
* Draw.io
* Epoch time
* Camel Case
