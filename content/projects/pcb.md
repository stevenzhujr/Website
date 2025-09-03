+++
title = "4. (2/2024) PCB Ornament"
slug = "PCB"
+++

This is my project creating a printed circuit board (PCB) ornament. This project uses Kicad and demonstrates understanding of the circuitry design process.

### Abstract

This is a guided project done in collaboration with IEEE. The main goal of this project is to familiarize myself with PCB and hardware design.

### Process
The process for designing basic circuitry requires three major steps:

1. Understanding the digital logic for a phenomenon

2. Implemnting and rendering it digitally using an app

3. Printing the board and assembling the components

### Design

***Goal***
The goal of the ornament is to make an ornament for Christmas. To achieve this, the PCB is designed to flash lights in a pattern across nine LEDs on a snowflake shaped PCB. The speed of the pattern should be able to be controlled.

***Implementation***
The pattern will increment through a counter, the pattern will have three stages, thus the counter will count up to three and reset. Then, through a timing chip and capacitors and a potentiometer, we can control how fast the pattern progresses. We do this through manipulating how fast the capacitors discharge through changing the resistance of the potentiometer.

This allows us to wire different patterns of lights to different stages of the counter, thus as it increments up, it appears as though the lights are shining in a pattern.

***Materials***
PCB board
Coin batteries
Resistors (any is fine as long as it fits the LED's requirements, can be surface mount or through hole resistors)
2 Capacitors (0.1 and 10 microFarads)
9 surface mount LEDs
Potentiometer
Switch
CD4017BE chip (counter)
SE555P chip (timer)

### Tools

The design of the PCB was done in KiCad, and the board was printed through OSH Park. All other materials were provided by IEEE and assembled by me through soldering.


### KiCad design
The specifics of the circuit logic is found here in the schematics:
{{< figure src="/images/PCB_KiCad.png">}}

An early board is design is as shown, the shape of the board can be modified and parts can be shifted as I did later:
{{< figure src="/images/PCB_Board.png">}}

### Demo
{{< vimeo_simple "915563729?share=copy" >}}