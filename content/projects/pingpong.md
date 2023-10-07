+++
title = "Ping pong"
slug = "pingpong"
+++

The Ping pong Rapid Defence Turret Repeater(PRDTR), is a ping pong ball launcher that was the subject of my ECE 5 course. Me and two other classmates, Vihan Jayaraman, and Jerry Wang, created this as our final project.

### Abstract

The main goal of our project was to construct a device that would be able to shoot projectiles with multiple degrees of freedom. We mounted a ping-pong ball launcher on a tiltable mount, giving it 360 degrees of coverage as well as the ability to change the angle of aim. Using a wirelessly connected PS4 controller, we send commands to the arduino’s serial monitor, which will rotate and tilt the turret accordingly as well as fire our ping-pong balls. 

### Technical Details

**Software**: Using AntiMicroX, we mapped the PS4 controls to keyboard commands. Afterwards, we used a serial monitor emulator, PuTTY in order to ensure every keyboard command was immediately sent to the arduino. The arduino then reads the keyboard commands from PuTTY and executes them.

**Hardware**: The entire system is powered using a 12V power supply. We designed a mosfet circuit to act as a switch for the spindle motors and used the enabler pins on the motor driver to control current to the Nema 17 stepper motors. 

### Equipment
- Arduino Uno
- 12V power supply adapter
- 2x Nema 17 Stepper Motors 
- 2x L298N motor drivers
- 2x 5.9V DC Spindle Motor
- SG90 micro servo motor
- PS4 Controller
- Rubber Bands
- Access to a 3D Printer

### Acknowledgements:
- Professor Theogarajan (the best professor)
- ECE TA’s
- IEEE
- Daniel Van Delsem
- Isaac879 on GitHub
- lmjd14 on Reddit
- William Ni for 3D Printing
- Owen Liu for electronics

We took heavy inspiration from an online [arduino lab](https://projecthub.arduino.cc/GordPayne/arduino-ping-pong-ball-cannon-abb8b3), with a design very similar in terms of mechanics, though we modified the desing with CAD so that it is 3-D printable.

### Presentation
{{<youtube ZhUitiKttmc>}}

### Full report
{{< figure src="/images/pingpong1.jpg">}}
{{< figure src="/images/pingpong2.jpg">}}
{{< figure src="/images/pingpong3.jpg">}}
{{< figure src="/images/pingpong4.jpg">}}
{{< figure src="/images/pingpong5.jpg">}}
{{< figure src="/images/pingpong6.jpg">}}
{{< figure src="/images/pingpong7.jpg">}}
{{< figure src="/images/pingpong8.jpg">}}