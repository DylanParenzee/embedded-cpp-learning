# Development Log

This is my dated engineering journal. Entries describe work I've actually completed; planned steps are labelled separately.

## 15 November 2026 — ESP32-S3 initial setup and TFT power test

**Hardware:** Freenove ESP32-S3 board, 2.8-inch SPI TFT touchscreen, multimeter.

- Verified approximately 3.3V between the ESP32's 3.3V and GND pins.
- Connected the TFT power and ground, then enabled its backlight through the LED pin. The display illuminated white.
- Installed Espressif ESP32 board support in Arduino IDE and selected the ESP32-S3 board.
- Uploaded my first ESP32 sketch using `Serial.begin(115200)` and repeated `Serial.println()` messages.
- Confirmed readable recurring output in Serial Monitor after checking serial configuration.

**What I learned:** A successful upload and readable serial output are separate checks. The TFT backlight can work before graphics communication is set up.

**Next:** Verify the exact TFT controller and wiring, connect SPI and display the first graphics.

## 29 October 2026 — Button-controlled LED: first completed structured lesson

**Hardware:** Arduino Uno R3, pushbutton, LED.

- Wrote and iteratively debugged a sketch using `pinMode()`, `digitalRead()`, `digitalWrite()` and `if/else`.
- Used `INPUT_PULLUP`, so the unpressed button reads HIGH and pressing it connects the input to GND and reads LOW.
- Physically verified the LED turned off, on and off again as the button was released, pressed and released.
- Explained the input logic and output control in my own words.

**What I learned:** Digital inputs and outputs, active-low button wiring and conditional logic.

## Late October 2026 — Ultrasonic-controlled servo demonstration

**Hardware:** Arduino Uno R3, HC-SR04 ultrasonic sensor, servo.

- Built a working simulation of a bin lid triggered by an object within roughly 25 cm.
- Moved the servo about 90 degrees and included a four-second delay to simulate time to place rubbish in the bin.
- Investigated a sensor that initially worked but stopped reliably detecting objects after the target moved away.
- Replaced the ultrasonic sensor; the issue was resolved.

**What I learned:** Combining sensor readings with actuator control, and checking hardware faults before assuming a software fault.
