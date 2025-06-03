The SparkFun AS7343 Python Package is based off the Arduino library for the sensor to get users started with example code for the AS7343. It works for Python, MicroPython and CircuitPython so you can choose which "flavor" of Python to use. This section goes over how to install the package in each supported Python environment along with the necessary tools for installation and running examples.

## Python Installation

For users on a Linux-based system (Raspberry Pi, etc.), install this package in Python with PyPi using the `pip3` command with the following steps:

* Set up a virtual environment from a specific directory using `venv`: `python3 -m venv path/to/venv (You can use any path here just remember to use the same one for each step).
* Install the Qwiic package: `path/to/venv/bin/pip3 install sparkfun-qwiic-as7343

That's it. Now you can run any example (or your own custom scripts) by running it with a command like: `path/to/venv/bin/python3 qwiic_as7343_ex1_basic_readings.py`

## MicroPython Installation

If you prefer to use MicroPython to run the examples on a microcontroller running MicroPython, follow these steps to install the package on your computer:

* Install [mpremote](https://docs.micropython.org/en/latest/reference/mpremote.html) on your computer.
* Connect the IoT RedBoard - ESP32 (or other MicroPython device) to your computer and install the package directly using mpremote mip: `mpremote mip install github:sparkfun/qwiic_as7343_py`
* Install the examples to the IoT RedBoard with the following mip command: `mpremote mip install github:sparkfun/qwiic_as7343_py@examples`

## CircuitPython Installation

Lastly, users who prefer CircuitPython can install the package with the following steps:

* Install [CircUp](https://docs.circuitpython.org/projects/circup/en/latest/#installation) on your computer.
* Make sure you have the latest version of the SparkFun Qwiic CircuitPython module installed with this command: `circup bundle-add sparkfun/Qwiic_py`
* Connect your CircuitPython device to your computer and install the package to the divice with circup: `circup install --py qwiic_as7343`

If you want to install specific examples from the repository, use the following command:

`
circup example qwiic_as7343\qwiic_as7343_ex1_basic_readings
circup example qwiic_as7343\qwiic_as7343_ex2_all_channels
circup example qwiic_as7343\qwiic_as7343_ex3_gain
circup example qwiic_as7343\qwiic_as7343_ex5_flicker_detection
circup example qwiic_as7343\qwiic_as7343_ex6_sleep
`

Note, the syntax used here are for Windows commands; Linux and Mac have different path separators. Refer to the [CircUp "example command documentation](https://learn.adafruit.com/keep-your-circuitpython-libraries-on-devices-up-to-date-with-circup/example-command) for more information.