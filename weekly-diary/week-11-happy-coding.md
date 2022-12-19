---
description: Coding on Arduino platform (POP-160)
---

# Week 11 - Happy Coding

November 4, 2022

Activity session 🏫 Date: 2022-11-04 08:50 Event: Class Venue: 1115 (11th Floor) Speaker(s): Aj. Jumpol

## Coursework (the 'what?') 🤷‍♂️

This week, we learned the Arduino language as well as how to connect circuits and jumper wires on Arduino boards. Embedded C++ used in Arduino is similar to C-like languages. In our code, we can call the C/C++ functions that make up the Arduino language. Since it's a subset version of C++ programming, it's simpler to write for C/C++ programmers. Unlike other microcontrollers, which can only run on Windows, Arduino is cross-platform, making it simple to run on any type of device. The Arduino IDE is used to create programs. We each have four assignments to complete in this class. It also provides support as a separate VS Code Extension, Cloud tool, IoT Hub, and Platform.IO support.

Here are some basic terms related to Arduino programming:

* **Setup**: The `setup()` function is run once when the Arduino is powered on or reset. It is used to initialize variables, pin modes, and other settings.
* **Loop**: The `loop()` function is run continuously after the setup() function has been completed. It is where you write the code that will be run over and over again.
* **Variables**: Variables are used to store data. They can be used to store numbers or strings of text.
* **Digital I/O**: Digital I/O is used to read and write data to digital pins on the Arduino.
* **Analog I/O**: Analog I/O is used to read and write data to analog pins on the Arduino.
* **Serial Communication**: Serial communication is used to send data between Arduino and other devices.
* **Libraries**: Libraries are code that has been written to make it easier to use certain functions on Arduino.

### Lab 1 - (LED Blink)

Our task is to set the LEDs to blink at various intervals. Therefore, in order to make the LEDs blink, we must fix the delay and experiment with the code.

Here's the sample Arduino code that can work with other microcontrollers using the Arduino framework.

```cpp
#define TIME_BLINK 750
#define LED_BLINK 2

void setup() {
  pinMode(LED_BLINK, OUTPUT);
}

void loop() {
  digitalWrite(LED_BLINK, HIGH); //ACTIVE LOW
  delay(TIME_BLINK);
  digitalWrite(LED_BLINK, LOW); //ACTIVE LOW
  delay(TIME_BLINK);
}
```

### Lab 2 - (Buzzer/Frequency Output)

This lab is a little different in that, depending on the coding, we can use the buzzer to create any song we desire.

```cpp
#define TIME_DELAY 500
#define PIN_BUZZER 9

void setup() {
  pinMode(PIN_BUZZER, OUTPUT);
}

void loop() {
 for(int i = 0; i < 500; i++) {
    digitWrite(PIN_BUZZER, HIGH);
    delayMicroseconds(TIME_DELAY); // maintain duty cycle
    digitWrite(PIN_BUZZER, LOW);
    delayMicroseconds(TIME_DELAY);
  }
  delay(500);
}
```

### Lab 3 - (Light Dependent Resistor)

An electronic component that is light-sensitive is an LDR. The resistance alters as light strikes it. Therefore, in this lab, we must modify the code so that the resistance is around 3000.

```cpp
void setup() {
  pinMode(1, INPUT);
  Serial.begin(115200); // baud rate depends on the board-to-board
}

void loop() {
  int LDR = analogRead(1);
  Serial.println(LDR);
  delay(500);
}
```

### Lab 4 - (Display on Super LCD)

The sample code used in this lab is already described in the professor's lab manual. However, we were given the task of making the text go from the LCD's beginning to end and then loop back through the beginning after it was finished.

```cpp
#include <SoftwareSerial.h>
#define rxPin 3
#define txPin 2
//set up a new serial port
SoftwareSerial mySerial = SoftwareSerial(rxPin, txPin);

void setup() {
  //set txPin high
  digitalWrite(txPin, HIGH);
  delay(1000);

  //define pin modes for tx, rx pins:
  pinMode(rxPin, INPUT);
  pinMode(txPin, OUTPUT);

  //set the data rate for the serial ports
  mySerial.begin(9600);
  //say something
  mySerial.write(128);
  mySerial.write(129);
  mySerial.write(0xFE);
  mySerial.write(0x38);   //2 line display
  mySerial.write(0xFE);   //Send command
  mySerial.write(0xC0);   //Show on line 2

  delay(2000);
}

void loop(){
  mySerial.write(130);
  mySerial.print("CPE#36");
  mySerial.write(154);
  mySerial.print("     KMUTT    ");
  delay(500);
}
```

## Impact (the 'so what?') 🚀

Arduino boards and components are widely available and reasonably priced, making them a great choice for hobbyists and professionals alike. The boards are highly flexible, allowing users to easily add sensors, motors, and other components to create custom projects.

As computer engineers, it is inevitable that we will come into contact with Arduino and electronic circuits at some point. Even if we choose not to pursue specialist majors in electronic circuits, we may be able to mend faulty household equipment. And the irony is, it has a high chance of having Arduino-based technology (ATMEGA or Arduino programming).

## Reflections (the 'now what?') 🤔

I find it quite enjoyable to understand how electronic circuits operate and how the wiring should be done. We gained knowledge by studying the intricate details of how electronic devices operate and the proper coding techniques.

Additionally, IoT is currently popular, so perhaps that was a perfect opportunity to understand the fundamentals of coding and how to combine it with electronic circuits.

## Further reading (optional) 📄

#### Keynotes 📝

TODO: Scannings for Happy Coding notebook scribbles (from B5 notebook)

* Microprocessor & Microcontroller
* Arduino POP 168 (ATMega 16 -> mem size, 8-> 8-bit processor)
  * open-source electronics prototyping platform
  * intended for artists, designers, and hobbyists (anyone interested in interactive objects or environments.)
  * sensors -> controller (processor) -> actuators
* POP - Project kit components
  * KIT 1: contains interface PCB, breadboard, USB to RS232, power adapters (DC jack), ethernet (PoE) i.e. ethernet to two pin
  * KIT 2: Project board (AT Mega 168)
    * Ports (Port 0 to Port 15) e.g. P0 is two holes & also have alias (P0 - A0)
      * so, we have A0 - A7, D2 - D9, +5V and GND
      * D0 and D1 work for serial COMM with PC (as Tx and Rx)
* Process
  * Bootloader mode
  * Program mode
    * Press the BL switch and hold
    * Press the RESET switch and hold
    * Release the RESET switch and then the BL switch
    * _Now, you can upload the code._

Programming structure

* Embedded C++

```cpp
void setup( ) {
  // run once
}

void loop() {
  // run forever
}
```

Issue: `avrdude: stk500_recv(): programmer is not responding`

Labs:

1. Blink LED
2. Frequency output (Piezo Electric Speaker) P15 (D9) -> C1 (10 uF) -> +(speaker)- -> GND

```cpp
void setup() {
	pinMode(9, OUTPUT);
}

void loop() {
	for (int i = 0; i < 500; i++) {
		digitalWrite(9, HIGH);
		delayMicroseconds(500);
		digitalWrite(9, LOW);
		delay Microseconds(500);
	}
}
	
```

1. LDR control for LED
2. Display on SLCD

#### Resources 🎁

* Documentation: [http://www.inexglobal.com/downloads/POP168kit\_e.pdf](http://www.inexglobal.com/downloads/POP168kit\_e.pdf)
