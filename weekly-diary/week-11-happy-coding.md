---
description: Coding on Arduino platform (POP-160)
---

# Week 11 - Happy Coding

November 4, 2022

TODO: Scannings for Happy Coding notebook scribbles (from B5 notebook)

Activity session 🏫 Date: 2022-11-04 08:50 Event: Class Venue: 1115 (11th Floor) Speaker(s): Aj. Jumpol

#### Keynotes 📝

* Microprocessor & Microcontroller
* Arduino POP 168 (ATMega 16 -> mem size, 8-> 8-bit processor)
  * open source electronics prototyping platform
  * intended for artists, designers, and hobbyists (anyone interested in interactive objects or envs.)
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

#### New ideas 💡

* something new?

#### Resources 🎁

* Documentation: http://www.inexglobal.com/downloads/POP168kit\_e.pdf

### Reflections 🔮

What do you feel?

How do these fit with your current practice and understanding?

How will you incorporate any new understanding or skill you have learned into your day-to-day practice?

#### Impact 🚀

How the session turned out to be of value if it did?

#### Final Reflection 🔚

Have you identified any learning needs to look forward into your personal learning and development?

How might you address these?

### Additional Notes 📄

Anything extra you would like to add goes here.
