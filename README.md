# ESP32 RGB LED Colour Transition

## Project Overview

This project demonstrates basic embedded programming using an ESP32 microcontroller and an RGB LED.

The ESP32 was programmed using the Arduino IDE to smoothly transition between different colours by controlling the intensity of the red, green and blue channels.

---

## Objectives

- Learn basic ESP32 programming.
- Understand PWM signal generation.
- Control an RGB LED using software.
- Gain experience uploading and debugging firmware.

---

## Hardware Used

| Component | Quantity |
|-----------|----------|
| ESP32 Development Board | 1 |
| RGB LED | 1 |
| Resistors (220 Ohm) | 3 |
| Breadboard | 2 |
| M-M Wires | 4 |

---

## Software Used

- Arduino IDE
- Elegoo ESP32 Arduino Core

---

## Circuit Description

Each LED channel (Red, Green and Blue) was connected to a PWM-capable GPIO pin on the ESP32 through a current-limiting resistor.

The brightness of each colour channel was controlled using Pulse Width Modulation (PWM).

---

## Features

- Automatic colour transitions.
- Smooth fading between colours.
- Adjustable transition speed through software.

---

## Challenges Encountered

Initially, the ESP32 development board was not detected by the Arduino IDE because the USB-to-UART driver was not installed. After identifying the issue, the appropriate Silicon Labs USB driver was installed, allowing the serial port to be recognised by the IDE.

A second issue occured when selecting the target board. At first, the incorrect ESP32 package had been installed, which cause the **ESP32 Dev Module** option to be unavailable (greyed out) within the Arduino IDE. Installing the correct ESP32 board package resolved the problem and allowed successful code upload to the microcontroller.

---

## Skills Demonstrated

- Embedded C/C++
- Arduino IDE
- PWM control
- Circuit assembly
- Hardware debugging
- ESP32 development

---

## Future Improvements

- Add push-button colour selection.
- Implement Bluetooth control.
- Add Wi-Fi control through a web interface.
- Synchronise multiple RBG LEDs.

## Lessons Learned

- Importance of installing the correct USB drivers for microcontroller communication.
- Importance of selecting the correct board definition within the development environment.
- Understanding that successful embedded development depends on both hardware and software configuration.
- Developed troubleshooting and debugging skills related to development toolchains.

## Demonstration
A demonstration video of the RGB LED colour transitions is included in this repository as 'rgb_led_working.mp4'. 

## Circuit photos
![Circuit Photo 1](images/rgb_led_setup1.jpg)

![Circuit Photo 2](images/rgb_leb_setup2.jpg)