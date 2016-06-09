![CyberPlant_Mini](http://image.cyber-plant.com/var/resizes/CyberPlantMiniSeriesC.jpg?m=1459175705)

##CyberPlant pH Mini v3.0

pH metering with Automatic Temperature Compensation for Arduino Pro Mini, Arduino Uno, Arduino Mega, Raspberry Pi and other devices. The pH Mini supports the connection of a pH electrode with BNC and temperature sensor Pt100 / Pt1000 for temperature compensation of measurement. The pH Mini uses an I2C-compatible
serial interface and operates from a single power supply
ranging from 2.7V to 5.5V. Can use as Shield for Arduino Pro Mini. The CyberPlant pH Mini is perfect for automating hydroponic systems or aquariums, will be useful in laboratories or to collect data on the computer.

###Features:

- Power Supply: 2.7V to 5.5V
- Measuring Range pH: 0-14
- Accurate pH readings: ± 0.01 pH
- Temp sensor support: pt100/pt1000
- Accurate temperature readings:  ±0.1°C
- BNC Connector
- Can use as Shield for Arduino Pro Mini
- PCB Size : 33.02 mm×17.78 mm

### pH measurement

I2C pins of SDA (A4), SCL (A5), VCC and GND is compatible with the Arduino Pro Mini and duplicated at the end of the board for other connectivity options.
Connect the pH electrode to BNC connector. 
When first connecting send the reset command "0" to configure the microcontroller.
Then calibrate first the isopotential point (pH 7.00 or 6.86) and then skew electrode (pH 4.00, 9.18 or 10.00).

![pH to I2C](http://image.cyber-plant.com/var/resizes/PHminiBaner1.jpg?m=1458074438)


**Sample code:** [*PhMeasurementSerial.ino*](https://github.com/cyberplantru/pH-Mini-v30-sample-code/blob/master/PhMeasurementSerial/PhMeasurementSerial.ino)

In sample code was used in one touch calibration sensor function.

### pH and Temp measurement

Switch between the temperature and pH sensors is available through the SPI interface. Sensors reading at alternately via I2C bus.

SPI headers pin SCLK (D13), SDI (D11) and CSB (D10) compatible with Arduino Mini. 

For automatic temperature compensation solder a 100 ohm resistor (blue) and connect a Pt100 temperature sensor. The 3-step measurement can reach a precision as high as ±0.1°C


**Sample code:** [*PhAndTempMeasurementSerial.ino*](https://github.com/cyberplantru/pH-Mini-v30-sample-code/blob/master/PhAndTempMeasurementSerial/PhAndTempMeasurementSerial.ino)

### Galvanic Isolation

To eliminate electrical noise use [I2Ciso Module](https://github.com/cyberplantru/I2C-iso/). 
Also I2C*iso* is needed for measurement of pH and Conductivity together in a same reservoir.

![pH to I2C](http://image.cyber-plant.com/var/resizes/PHminiBaner3%2Cjpg.jpg?m=1458077695)


----------

### Package include:
-     1 x pH Mini v3.0
-     2 x 12 PLS connectors
-     1 x 4 angle PLS
-     2 x 4k7 resistors
-     1 x 100R 0.01% resistor

----------

### Documentation:

- [Hardware](https://github.com/cyberplantru/pH-Mini-v30-hardware/)
- [link to CyberPlant](http://www.cyber-plant.com).
