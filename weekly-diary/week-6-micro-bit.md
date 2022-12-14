---
description: Learning about a versatile microcontroller
---

# Week 6 - micro:Bit

September 23, 2022

MicroBIT - Many programming options (I prefer Python and JavaScript over MakeCode or drag and drop coding program developed in MIT called Scratch).

## Coursework (the 'what?') 🤷‍♂️

The focus of week 6 is becoming familiar with the features and operation of the Micro:bit. It is an open-source ARM-based educational embedded system. Let's take a quick recap of MicroBit specifications:

| Name         | BBC micro:Bit                                                                                                                   |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------- |
| CPU          | v2: Nordic nRF52833, 64 MHz [ARM Cortex-M4](https://en.wikipedia.org/wiki/ARM\_Cortex-M4) core, 512 KB Flash, 128 KB RAM        |
| Connectivity | [Bluetooth LE](https://en.wikipedia.org/wiki/Bluetooth\_LE), [MicroUSB](https://en.wikipedia.org/wiki/MicroUSB), edge connector |
| Release date | v2: 13 October 2020                                                                                                             |

<figure><img src="../.gitbook/assets/image (9) (1).png" alt=""><figcaption><p>source: <a href="https://microbit.org/get-started/user-guide/overview/">https://microbit.org/get-started/user-guide/overview/</a></p></figcaption></figure>

The Micro:bit is a portable computer that shows us how hardware and software interact with each other. It has few buttons, many sensors, an LED 2D display matrix, and other programmable I/O functions. The micro:bit also has built-in temperature and light sensors, as well as connectors around the bottom that can be used to add extras, since it has adequate GPIO ports.

It can be programmed using a USB connector and desktop, but also by pairing it to tablet/mobile devices via Bluetooth. The coding process is way too convenient. Additionally, it has two programmable buttons and 25 LED lights, which can be utilized for countless possibilities. Creative ideas are still there to be developed regarding microcontrollers.

## Impact (the 'so what?') 🚀

It is a well-rounded board to explore electronics, prototyping, testing, and coding with a gamified experience. The micro:bit can be configured to perform a variety of tasks, including acting as a game controller, a digital watch, and a home security monitor. Therefore, we may utilize the micro:bit for a variety of tasks and can adapt them to employ them in projects to control the actions and performances of small robots.

## Reflections (the 'now what?') 🤔

Using micro: Bit, we can delegate the burden of electronics setup and work with different sensors and the bus system they support (CAN, I2C, SPI). Rather than these, we can opt to learn cooperation, communication, and design thinking.

## Further reading 📄

Fun fact: micro bit also supports Zephyr RTOS. Using this we can build industrial-grade IoT applications just from an education-purpose-built microcontroller platform.

But for practical reasons (rather than Arduino (AVR), or micro:Bit) based system which is beginner level and targeted to most learners, I opt for using a sophisticated microcontroller platform for the prototyping related works to overcome computational constraints and limitations possessed by these board. My primary choice is using an Espressif-based system (ESP8266, ESP32) or STMicroelectronics-based STM32 implementations.

Here is an example from my practice sessions demonstrating different programming setups on an ESP-32 microcontroller (PlatformIO - ESP IDF and Arduino framework + Arduino IDE).

{% embed url="https://www.youtube.com/watch?ab_channel=YuilTripathee&v=uMiHQFgmsrE" %}
source: My own personal work
{% endembed %}

### References 🔖

* [Micro:bit Educational Foundation | micro:bit](https://microbit.org/)
* [iBIT-RacerE\_210626-re.pdf](https://inex.co.th/store/manual/eng/iBIT-RacerE\_210626-re.pdf)
* [Micro Bit - Wikipedia](https://en.wikipedia.org/wiki/Micro\_Bit)

Additional ways to program a micro:Bit

* [Tinkercad Blog: Python Coding with micro:bit in Tinkercad Circuits | Tinkercad](https://www.tinkercad.com/blog/python-coding-with-microbit-in-tinkercad-circuits)
* [Tinkercad Blog: Explore Micro:bit With Tinkercad | Tinkercad](https://www.tinkercad.com/blog/explore-microbit-with-tinkercad)
* [BBC micro:bit — PlatformIO v6.1 documentation](https://docs.platformio.org/en/stable/boards/nordicnrf51/bbcmicrobit.html)
* [How can I code in C++ using the micro:bit : Help & Support](https://support.microbit.org/support/solutions/articles/19000017961-how-can-i-code-in-c-using-the-micro-bit)
* [BBC Micro:bit C++ Getting Started : 7 Steps - Instructables](https://www.instructables.com/BBC-Microbit-C-Getting-Started/)
* [Python Editor for micro:bit](https://python.microbit.org/v/beta)
* [Microbit with Gobot](https://gobot.io/documentation/platforms/microbit/)
* [BBC MicroBit V2 — Zephyr Project Documentation](https://docs.zephyrproject.org/latest/boards/arm/bbc\_microbit\_v2/doc/index.html)
* [BBC micro:bit V2 — PlatformIO latest documentation](https://docs.platformio.org/en/latest/boards/nordicnrf52/bbcmicrobit\_v2.html)

Expert review of micro:Bit board:

* [micro:bit for Robotics - YouTube](https://www.youtube.com/watch?v=iwaRidlm2RM\&ab\_channel=KevinMcAleer)
* [BBC micro:bit v2 Review! : A Good Recommendation? - YouTube](https://www.youtube.com/watch?v=QHiXLPorrF4\&ab\_channel=Robu.in)
* [102110408 Seeed Technology Co., Ltd | คอมพิวเตอร์แบบฝัง | DigiKey](https://www.digikey.co.th/th/products/detail/seeed-technology-co.,-ltd/102110408/16680580)

