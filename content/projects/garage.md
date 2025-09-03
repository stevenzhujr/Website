+++
title = "6. (6/2024) Garage Door"
slug = "garage"
+++

The Garage Door was the final assignment of my ECE 153B course. I produced created the door with another classmate, Vihan Jayaraman.

### Abstract

The main goal of our project was to construct a device that models a garage door. The door has to be controlled by both temperature and remote input. The position of the door has to be sensed by an accelerometer and the remote input has to be done through a bluetooth module.

### Behavior

The garage door would open at a set temperature and closed at a set temperature, say 30 and 15 degrees celsius. The garage door would also open and closed pased on remote input through a computer. The remote input supercedes the temperature control, the remote overide lasts for 30 seconds, afterwhich the door will once again listen to temperature inputs. 

We check the garage door's position through an accelerometer attached to it. All sensors and motors are connected via breadboard, but the computer input is sent over the bluetooth module and is not connected directly to the stm32l4 board. 

### Technical Details

**Software**: Using C, we coded the stm32l4 to communicate with the bluetooth module, temperature sensor, and motor using I2C, SPI, and UART repsectively. We used uVision by Keil for embedded coding and used Termite for remote input.

**Hardware**: The entire system is powered using a 5V power supply. We used a cardboard box to construct the main body of the garage door. With a 3-D printed lever arm we connected the stepper motor to the garage door. Using breadboard and wires we connected the sensors and motor to the stm32l4 board.

### Code
Find the code for this project here: https://github.com/stevenzhujr/153B-final

### Equipment
- stm32l4
- 55V power supply adapter
- 28BYJ-48 5V Stepper Motor
- ULN2003 Step Motor Driver Board
- HiLetgo HC-06 RS232 4 Pin Wireless Bluetooth Serial RF Transceiver
- HiLetgo GY-291 ADXL345 3-Axis Digital Acceleration of Gravity Tilt Module for Arduino
- Breadboard
- 3-D printed lever arm
- Paper pin
- Rubber Bands
- Cardboard box