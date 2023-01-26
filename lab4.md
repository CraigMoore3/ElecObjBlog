# Lab 4 - Analog Inputs on UNO R3 - January 26, 2023

Covering the basics of using analog inputs with the Uno R3

## Prep

* I started this lab by familiarizing myself with some vocabulary. The [Sparkfun](https://learn.sparkfun.com/tutorials/serial-communication/all) website has a great tutorial outlining the difference between Serial and Parallel interfaces- the latter sends bits of data sequentially, one after the other, while the former uses an array of wires to transport. I found the following schematic very helpful in visualizing this process.

[Visualization of Serial Communication](images/serialComGraph.png)

* With a deeper understanding of the vocabulary, I read over the entire lab doccument again before getting to work on the first excercise.

### 1: Serial Output

* I copied the code from the lab doccument, built it and uploaded it without any problems. 

[Screenshot of Excercise 1 code](images/l4e1SerialOutputCode.png)

* The Serial Monitor printed "hello!" once per second.

[Screenshot of Serial Monitor printing "hello!"](images/l4e1SerialMonitorHello.png)

* Taking the time to study each of the functions in the code, I took note of a new term/unit: **Baud Rate:** Unit of measurement for symbol rate, in this case, 9600 bits per second. I still have more questions about this, but for the sake of the lab, an intuitive understanding will do.

### 2: Voltage Divider

* To assist with the process of rebuilding a voltage divider, I was able to refer back to my previous blog post for guidance, imagine that!

* I opted to build the voltage divider using two 1k ohm resistors.
  
[Photo of Voltage Divider breadboard layout](images/l4e2Breadboard.png)

* With the breadboard built out, I copied the code, taking the time to add my own notes in an effort to understand what it's doing.
  
[Screenshot of Voltage Divider Code](images/l4e2VoltDivCode)

* After building and uploading, I had what looked like success, although I couldn't be sure until I converted the analog reading to volts.

[Screenshot of Voltage Divider Serial Monitor](images/l4e2SerialMonitor)

#### 2.5: Showing Volts Instead

* I copied the new "float" line of code and moved it around until I found the right place for it, which was after "reading" was initialized, but before the Serial Monitor is told to print "voltage"
  
[Screenshot of modified code to convert to Volts](images/l4e25Code.png)

* With the new conversion code installed, I uploaded it to the controller and had success.

[Screenshot of Serial Monitor displaying accurately divided voltage (2.5)](images/l4e25SerialMonitor.png)

* Finally, I copied the print code to display both "reading" and "voltage" in the Serial Monitor
  
[Screenshot of modified code to display "reading" and "voltage"](images/l4e252Code.png)

[Screenshot of Serial Monitor displaying both "reading" and "voltage" values](images/l4e252SerialMonitor.png)

* From what I can gather, println is used to finalize a list of print requests. I think it means "print line"

### 3: Potentiometer

* I started by modifing my breadboard to use a potentiometer instead of resistors

[Photo of voltage divider breadboard using a potentiometer](images/l4e3Breadboard.png)

* Uploading the same code as in Excersise 2.5, the Potentiometer Voltage Divider worked on first try. It was turned all the way down to start. I turned it all the way up, then gradually reduced it to zero as seen in the Serial Monitor
  
[Screenshot of Serial Monitor displaying a decreasing range of voltage values](images/l4e3SerialMonitor.png)

### 4: Controlling the Brightness of an LED

### 5: Light Sensor

## Process

## Results

## Conclusion
