

## Power Consumption Tips

The AS7343 boasts some impressively low power consumption numbers but the breakout board includes a few extra components that increase the total draw of the breakout. In our testing, the red Power LED is the biggest culprit and disabling it reduces total current consumption by roughly 300&micro;A. For example, opening the LED jumper to disable the LED drops current while idle from ~320&micro;A down to ~3&micro;A. 

Also, the on-board white LED defaults to draw 4mA from the AS7343's LED Drive pin while active so we recommend turning it on only when needed for spectral sensing. This is the *lowest* setting for the LED drive pin and can be adjusted to up to 12mA in both the Arduino library and Python package. Refer to the AS7343 [datasheet](./assets/component_documentation/AS7343_DS001046_6-00.pdf) for more information on driving an external LED.

## General Troubleshooting

!!! info
    <p><span class="glyphicon glyphicon-question-sign" aria-hidden="true"></span> <strong>Not working as expected and need help? </strong></p>
    <p>If you need technical assistance and more information on a product that is not working as you expected, we recommend heading on over to the <a href="https://www.sparkfun.com/technical_assistance">SparkFun Technical Assistance</a> page for some initial troubleshooting.</p>
    <center>
    [SparkFun Technical Assistance Page](https://www.sparkfun.com/technical_assistance){ .md-button .md-button--primary }
    </center>
    <p>If you can't find what you need there, you'll need a <a href="https://forum.sparkfun.com/ucp.php?mode=register">Forum Account</a> to search product forums and post questions.<p>