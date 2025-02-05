# IoT-GoodMorning: Subproject Weather

## Goals of the Subproject
-Provide and publish live weather data. 


## List of Requirements Group03
 * Publish random values to broker with Raspberry PI
 * Get analog readout from KY-018 to RPI via i2c Bus
 * Publish analoge readout to broker
 * Subscribe topic to control LED
 
## Overview Hardware System
* Raspberry PI 3
* XXX
* KY-018 Light Dependat Resistor (LDR)

## Preparation for Startup
* install **paho client** with ``sudo pip install paho-mqtt``
* install **adafruit i2C ADC** with ``sudo pip3 install adafruit-circuitpython-ads1x15``

## Get / control values
* To control LED, publish value x to brokertopic Greenhouse/Light/LED_Status
  ``x = 1 : LED On |
  x = 0 : LED Off``
* Brightness values get published at Greenhouse/Light/Brightness
* 
## Hardware routing
![signal routing](https://user-images.githubusercontent.com/94985537/149324416-230a03ea-fdb1-4d14-bd33-b21e2e305ccc.png)

##  Developers and authors Subproject
 * Andreas Lazar
 * Philip Seitz
 * Kevin Maass
 * Nico Sander
 ## Shopping List
 *LED RING
 *https://www.reichelt.de/entwicklerboards-neopixel-ring-mit-12-ws2812rgb-leds-debo-led-np12-p235468.html?&trstct=pos_0&nbc=1
 
 *LIGHT SENSOR
 *https://www.reichelt.de/entwicklerboards-digitaler-lichtsensor-bh1750-debo-bh-1750-p224217.html?&trstct=pos_6&nbc=1

