Let's take a closer look at the examples included in the SparkFun AS7343 Arduino Library. This section assumes users are following the assembly instructions from the Hardware Assembly/Qwiic Start sections and are using a SparkFun RedBoard IoT - ESP32.

## Example 1 - Basic Readings

The first example sets up the AS7343 to operate with default settings and outputs data from just four channels (Red, Green, Blue and NIR). Open the example in Arduino by navigating to **File** > **Examples** > **SparkFun AS7343 Arduino Library** > **Example_01_BasicReadings**. Next, select your board (RedBoard IoT - ESP32) and Port and click the "Upload" button. After the code finishes compiling and uploading, open the [serial monitor]() with the baud set to **115200** and you should see readings for red, blue, green and NIR print out like the screenshot below shows:


## Example 2 - All Channels

Example 2 - All Channels shows how to set up the AS7343 with default settings to print out all spectral data from the sensor. This example is nearly identical to the first outside of the serial data printed out. Instead of getting and printing data from four specific channels, this example requests data from all channels and prints it as comma separated values. The data follows the format of **value needed**. Open the example in Arduino by navigating to **File** > **Examples** > **SparkFun AS7343 Arduino Library** > **Example_02_AllChannels**. 

## Example 3 - Gain

The third example shows how to set up the AS7343 with specific Spectral Engines Gain Settigns (aka AGAIN) and cycle through the gain settings using serial commands. Open the example in Arduino by navigating to **File** > **Examples** > **SparkFun AS7343 Arduino Library** > **Example_03_Gain**. If necessary, select your board and port and click the "Upload" button. Open the serial terminal with the baud set to **115200** after the code finishes uploading. 

## Example 4 - Interrupt

The fourth example demonstrates how to set up the AS7343's interrupt pin to fire when 

## Example 5 - Flicker Detection

## Example 6 - Sleep

## Example 7 - Web Terminal Bar Graph

## Example 8 - GPIO