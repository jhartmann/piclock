# piclock

## Overview
piclock is an alarm clock written in Micropython for Raspberry Pi Pico WH.

## Features
 - Alarm clock with an infinite number of alarm times
 - Alarm on/off
 - Snooze function
 - Displaying day of week and day of month
 - Displaying temperature and humidity
 - Display off / standby mode

## Parts
|Count|Part                                                              |
|-----|------------------------------------------------------------------|
|1    |Raspberry Pi Pico WH Microcontroller                              |
|1    |8x32 LED Matrix Display MAX7219                                   |
|3    |Buttons                                                           |
|1    |DHT-22 Sensor                                                     |
|4    |Resistors 10k (3 pull-up for the buttons, 1 for the DHT-22 sensor)|
|1    |Piezo buzzer, active                                              |

## Pinout
|Part       |Connection |RPi Pico |Connection|
|-----------|-----------|---------|----------|
|Button bn0 |S0         |27       |GP21      |
|           |S1         |36       |3V3(OUT)  |
|           |10k        |28       |GND       |
|           |           |         |          |
|Button bn1 |S0         |29       |GP22      |
|           |S1         |36       |3V3(OUT)  |
|           |10k        |28       |GND       |
|           |           |         |          |
|Button bn2 |S0         |32       |GP27      |
|           |S1         |36       |3V3(OUT)  |
|           |10k        |28       |GND       |
|           |           |         |          |
|Buzzer     |S          |34       |GP28      |
|           |+          |36       |3V3(OUT)  |
|           |-          |23       |GND       |
|           |           |         |          |
|Matrix LED |CLK        |24       |GP18      |
|           |DIN        |25       |GP19      |
|           |CS         |22       |GP17      |
|           |VCC        |40       |VBUS      |
|           |GND        |23       |GND       |
|           |           |         |          |
|DHT22      |DATA       |19       |GP14      |
|           |VCC        |36       |3V3(OUT)  |
|           |GND        |23       |GND       |
|           |           |         |          |