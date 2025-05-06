In this Quick Start Guide we'll connect the SparkFun Spectral Sensor Breaout - AS7343 (Qwiic) to an IoT RedBoard - ESP32 to output measurements of visible and near-infrared light and display them in a colorful web terminal bar graph.

If you're not familiar with using sensor breakouts, development boards or the development environments covered in this guide, refer to the [Hardware](./hardware_overview.md) & [Software]() sections of this Hookup Guide for a detailed overview of the board along with instructions on setting up and using the SparkFun AS7343 Arduino Library and MicroPython package.

## Basic Assembly

As this is a Qwiic breakout, assembling the circuit only requires connecting the sensor breakout to a Qwiic-compatible development board like the IoT RedBoard - ESP32. Connect the Spectral Sensor Breakout to the IoT RedBoard with a Qwiic cable and then connect the IoT RedBoard to your computer with a USB-C cable like the photo below demonstrates:



## Software Setup

The IoT RedBoard - RP2350 comes pre-loaded with MicroPython firmware so users who want to run the example in MicroPython can move on to the Example section below. Arduino requires installing the proper board definitions for the IoT RedBoard - RP2350 (or alternate Arduino dev board of your choosing).

### SparkFun AS7343 Arduino Library

Install the SparkFun AS7343 Arduino library with the [Arduino Library Manager](https://docs.arduino.cc/software/ide-v1/tutorials/installing-libraries/) and search for "SparkFun AS7343". Make sure to install the latest release.

### IoT RedBoard Definitions

The IoT RedBoard - ESP32 is included in the ESP32 boards package from espressif. Install the boards package in the [Arduino Boards Manager](https://docs.arduino.cc/software/ide-v2/tutorials/ide-v2-board-manager/) by searching for "ESP32" and install the latest version.

### SparkFun AS7343 MicroPython Driver



## Web Terminal Bar Graph Example

The bar graph examples for both Arduino & MicroPython set up the AS7343 to output from all channels and format the data so the web terminal can read it and display it in a bar graph. The Web Terminal Bar Graph example requires 

## Arduino Example

* Open "Example 7 - Web Terminal Bar Graphs" in Arduino and select your board (IoT RedBoard - ESP32) and Port.