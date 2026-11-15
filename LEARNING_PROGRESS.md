# Learning Progress

This record separates **encountered** topics from those I've **explained or demonstrated**. It isn't a claim of professional proficiency.

| Concept or skill | Status | Evidence / next step |
| --- | --- | --- |
| Arduino `setup()` and `loop()` | Explained in my own words | Explained one-time initialisation versus repeated execution after the ESP32 test |
| Digital input and output | Demonstrated | Built and tested a pushbutton-controlled LED |
| `INPUT_PULLUP` and active-low logic | Explained and demonstrated | Explained HIGH when released, LOW when pressed; tested physical circuit |
| `if/else` control flow | Demonstrated with guidance | Used to control LED from button state |
| Ultrasonic sensing and servo actuation | Demonstrated in a guided build | Working bin-lid simulation |
| Hardware troubleshooting | Demonstrated | Isolated a faulty ultrasonic sensor by replacement |
| Multimeter DC voltage measurement | Practised | Measured the ESP32 3.3V supply |
| ESP32-S3 upload and Serial Monitor | Practised successfully | Uploaded sketch and observed repeated serial messages |
| SPI communication | Planned | Not yet wired or tested for this display |
| TFT graphics and touch input | Planned | Backlight only confirmed; no graphics or touch test yet |
| General C++ proficiency | In development | Continue writing original code and explaining design choices |

## Revision notes

- Keep practising C++ syntax and writing sketches without relying on complete examples.
- Distinguish a display's backlight power from the communication needed to draw pixels.
- Continue building a repeatable troubleshooting process: observe, isolate, test, confirm.

## Working principles

I want to understand why something works rather than just copy code. For future entries, I'll note whether I wrote the solution independently, needed hints or followed a worked example.
