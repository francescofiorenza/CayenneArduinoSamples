# Cayenne Thermistor Example

This sketch shows how to send temperature data to a Thermistor Sensor in the Cayenne Dashboard.

###### Steps:
1. In the Cayenne Dashboard add a new Thermistor widget.
2. Set the widget to Value Display.
3. Select Virtual Pins and a virtual channel number.
4. Set VIRTUAL_CHANNEL to the channel number you selected.
5. Attach a thermistor to an analog pin on your Arduino. Make sure to use an analog pin, not a digital pin.
   * Schematic:
   ```
   [Ground] -- [10k-resistor] -- | -- [Thermistor] -- [5V]
                                 |
                             Analog Pin
   ```
6. Set the thermistorPin variable to match the pin used to connect the thermistor.
7. Set the token variable to match the Arduino token from the Dashboard.
8. Compile and upload this sketch.
9. Once the Arduino connects to the Dashboard it should automatically update the Thermistor widget with data.