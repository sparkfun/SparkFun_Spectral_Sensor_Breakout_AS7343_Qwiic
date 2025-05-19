Let's take a closer look at the examples included in the SparkFun AS7343 Arduino Library. This section assumes users are following the assembly instructions from the Hardware Assembly/Qwiic Start sections and are using a SparkFun RedBoard IoT - ESP32.

## Example 1 - Basic Readings

The first example sets up the AS7343 to operate with default settings and outputs data from just four channels (Red, Green, Blue and NIR). Open the example in Arduino by navigating to **File** > **Examples** > **SparkFun AS7343 Arduino Library** > **Example_01_BasicReadings**. Next, select your board (RedBoard IoT - ESP32) and Port and click the "Upload" button. After the code finishes compiling and uploading, open the [serial monitor]() with the baud set to **115200** and you should see readings for red, blue, green and NIR print out like the screenshot below shows:


## Example 2 - All Channels

Example 2 - All Channels shows how to set up the AS7343 with default settings to print out all spectral data from the sensor. This example is nearly identical to the first outside of the serial data printed out. Instead of getting and printing data from four specific channels, this example requests data from all channels and prints it as comma separated values. Open the example in Arduino by navigating to **File** > **Examples** > **SparkFun AS7343 Arduino Library** > **Example_02_AllChannels**. 

In order to get data from all channels, the AS7343 takes measurements in three cycles with each one stepping through four individual channels combined with readings from the Clear/VIS and Flicker Detect/FD which is then stored in the sensor's data registers. The example prints out spectral data stepping through each channel from 0 to 17 following the format of **value needed**.

## Example 3 - Gain

The third example shows how to set up the AS7343 with specific Spectral Engines Gain Settigns (aka AGAIN) and cycle through the gain settings using serial commands. Open the example in Arduino by navigating to **File** > **Examples** > **SparkFun AS7343 Arduino Library** > **Example_03_Gain**. If necessary, select your board and port and click the "Upload" button. Open the serial terminal with the baud set to **115200** after the code finishes uploading. 

The example accepts serial inputs of "+" and "-" to step up and down, respectively, through the available gain settings and prints out the value of the gain each time it's updated.

## Example 4 - Interrupt

The fourth example demonstrates how to set up the AS7343's interrupt pin to fire when values from a specific channel exceed a specified limit. The example defaults to watch channel FZ (450nm aka Blue) and trigger the interrupt when it reports values over 10 counts. 

## Example 5 - Flicker Detection

Example five shows how to set up and monitor flicker detection readings from the sensor. It sets up the AS7343 with default settings with flicker detection enabled and prints the values over serial.

## Example 6 - Sleep

Example six shows how to put the AS734 in and out of Sleep Mode to take intermittent measurements.

## Example 7 - Web Terminal Bar Graph

The seventh example takes data from all of the AS7343's channels (visible spectrum, NIR and clear) and formats it in a way to work with the SparkFun Online Serial Terminal to display the readings in a colorful bar graph. 