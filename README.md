# CO2Ampel
A device for visual representation of  CO2 concentraition in the air. Helps monitoring air quality in order to reduce the risk of COVID19 infections in closed rooms.

![Photo](https://github.com/OpenInnovationLabKonstanz/CO2Ampel/raw/master/Documentation/co2_1.jpg )

## Project Overview



## Hardware

![Photo](https://github.com/OpenInnovationLabKonstanz/CO2Ampel/raw/master/Documentation/co2_3.jpg )

The device consists of a CO2ESP32-WROOM-32 as a main controller. 

### CO2 Sensor
Due to the bad availability of CO2 sensors during the COVID19 pandemic, multiple sensor types are supported.
* SenseAir S8 (UART)
* MH-Z19B (pin-compatible to the S8)
* Sensirion SCD30 (I2C)


### Environment Sensor
As an additional method of air quality measurement, a Bosch BME680 multi environmental sensor is used. 
It provides temperature, rel. humidity, air pressure and VOC (volatile organic compounds) measurement.

### Ambient Light Sensor
In order to adapt the display and LED brightness, a OPT3001 ambient light 


### Display
A 4-digit 7-segment display, driven by a TitanMicro TM1638 is used to display the current CO2 concentration (in ppm).


## PCB
The PCB is routed as a 2-layer PCB. Parts are only placed on the top side in order to facilitate mass production.
Layout files are provided as Eagle 6.4 .brd and .sch files.



## Software
The firmware for the ESP32 is written in Arduino, using the ESP32-Arduino support package.
It uses following external libraries:
* SparkFun SCD30 Library (ToDo: Link)
* ClosedCube OPT3001 Library (ToDo: Link)
* Adafruit Sensor Library (ToDo: Link)
* Adafruit BME680 Library (ToDo: Link)
* ...


## Mechanical
The housing is laser-cut from 3mm acrylic sheets. Use sheets with satin finish for better light dispersion (eg. TroGlass Satin).
DXF files for cutting and engraving are provided in *Mechanical*.


## Contact
Stefan Oechslein
Open Innovation Lab Konstanz
oil<at>htwg-konstanz.de