# Embedded C++ Learning

I'm learning C++ with a focus on embedded software engineering, using hands-on electronics projects to turn programming concepts into working hardware.

My background is in mechanical maintenance and fault diagnosis. I'm building on that experience as I learn to write software, understand microcontrollers, design basic circuits, and troubleshoot hardware and code together.

This repository is my learning record: what I've actually built, the problems I've encountered, and what I understand so far. It's a work in progress rather than a collection of polished tutorials.

## Learning goals

- Build a strong foundation in general-purpose C++ as well as embedded programming.
- Understand how microcontrollers interface with sensors, actuators and displays.
- Get comfortable reading datasheets, wiring circuits, testing and debugging.
- Work toward a facial-recognition door-lock project that brings together hardware, software and connectivity.

## Hands-on progress

| Exercise | Hardware | Current status |
| --- | --- | --- |
| Button-controlled LED | Arduino Uno R3, pushbutton, LED | **Completed and physically tested** |
| Ultrasonic-triggered servo / simulated bin lid | Arduino Uno R3, HC-SR04, servo | **Built and physically tested** |
| ESP32-S3 serial communication | Freenove ESP32-S3 | **Program uploaded; serial output verified** |
| SPI TFT touchscreen | ESP32-S3, 2.8-inch TFT module | **In progress — first full-screen SPI graphics test working** |

### Button-controlled LED

I wrote and debugged an Arduino sketch that reads a pushbutton configured with `INPUT_PULLUP` and controls an LED using an `if/else` condition. I tested the LED with the button released, pressed and released again. This was my first formally completed practical lesson.

### Ultrasonic sensor and servo

I built a small simulation of an automatic bin lid. When the ultrasonic sensor detected an object within about 25 cm, the servo moved roughly 90 degrees, paused for four seconds and then returned. One ultrasonic sensor became unreliable during testing; replacing it resolved the issue.

### ESP32-S3 and touchscreen

I configured Arduino IDE for a Freenove ESP32-S3 and uploaded a simple C++ serial-output program. After checking the serial settings, I was able to see the message repeat in Serial Monitor. I also used a multimeter to verify a 3.3V supply and got the 2.8-inch TFT backlight working. The first graphics test initially produced partial colour and static, but an alternative driver and corrected inversion settings produced a full-screen blue image. Touch input is still untested.

## Projects

I keep short learning exercises in this repository and give larger projects their own repositories, with source code, hardware documentation and an engineering log.

| Project | Status | Repository |
| --- | --- | --- |
| ESP32-S3 touchscreen interface | In progress: full-screen SPI graphics working; touch input next | [esp32-touchscreen-interface](https://github.com/DylanParenzee/esp32-touchscreen-interface) |
| RFID-controlled TV timer | Planned | Not started |
| Facial-recognition door lock | Long-term goal | Not started |

## Development journal

I keep a dated record of milestones, test results and troubleshooting in [CHANGELOG.md](CHANGELOG.md).

I track which concepts I've encountered versus what I can explain and demonstrate independently in [LEARNING_PROGRESS.md](LEARNING_PROGRESS.md).

## How I work

I try to write and troubleshoot the code myself, with guided feedback when needed. My notes reflect actual tests and lessons learned; I'll add source files, schematics, photos and short demonstrations as each project develops.

*Started October 2026 — ongoing.*
