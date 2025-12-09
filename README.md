# People-Counter
Embedded systems project using ESP32, IR sensors

A compact embedded systems project that uses a Heltec Wireless Stick V3 (ESP32‑S3) and a pair of IR break‑beam sensors to detect direction and count people moving through a doorway.
The device can run on a Li‑Po battery, supports LoRaWAN communication, and was built as part of coursework in embedded systems and IoT.

Features
ESP32‑S3 (Heltec Wireless Stick V3) programmed using Arduino/C++

Dual IR break‑beam sensors used for entry/exit direction detection

Non‑blocking timing logic using millis()

Debounce + noise filtering to avoid false triggers

OLED display for local count visualization

Optional LoRaWAN uplink for transmitting counts to the cloud

Serial Monitor debug tools

Breadboard prototype with clean wiring and soldered final version

Battery‑powered operation (Li‑Po 3.7V) for portable deployment

What This Project Demonstrates
This project demonstrates my practical skills in:

Embedded Programming
ESP32‑S3 development in Arduino

Writing non-blocking state machines

Handling ISR‑free digital sensor polling

Using I²C (OLED) and GPIO peripherals

Sensor Integration
Working with through‑beam infrared sensors

Debouncing and noise suppression

Direction detection with multiple sensing stages

Hardware Debugging
Diagnosing power issues (5V rail, Li‑Po input, USB power path)

Verifying sensor functionality with oscilloscope/serial output

Ensuring stable operation on a battery

Electronics Prototyping
Breadboard prototyping → final soldered harness

Choosing correct battery connectors (JST‑SH 1.25 mm)

Testing under real‑world doorway conditions

Simple System Design & Testing
Designing a complete embedded IoT flow

Measuring sensor accuracy and refining thresholds

Calibrating entry/exit logic to avoid double counts

Wiring Diagram
(Insert your Fritzing or hand‑drawn diagram here.)

Typical wiring summary:

IR Emitter → 5V, GND

IR Receiver → 5V, GND, OUT → ESP32 GPIO

Second IR pair → same as above on a different GPIO

OLED Display → SDA, SCL (I²C)

Battery → JST‑SH 1.25 mm connector on Heltec

Photos
(Add these when you have them):

Breadboard prototype

IR sensors aligned on a doorway

Heltec ESP32‑S3 with OLED showing live count

Final soldered version

Optional enclosure/build

Code
Your project files should live in a folder like:

/code/main.ino
/code/sensor_logic.cpp
/code/sensor_logic.h
Include:

Non‑blocking loop

State machine for entry/exit

LoRaWAN sender (optional)

OLED display code

Debug output

About Me
I am a Mechatronics Engineering student with a strong interest in embedded systems, IoT devices, and sensor technology. I enjoy building practical hardware projects that combine electronics, firmware, and wireless communication.
Currently, I am gaining hands‑on engineering experience while working in R&D at DIO‑IOT, where I focus on embedded development and prototyping.
