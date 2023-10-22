+++
title = "Ping pong"
slug = "pingpong"
+++

The Pingpong Rapid Defence Turret Repeater(PRDTR), or the Pingpong Ball Launcher project, was the final assignment of my ECE 5 course. I produced the launcher with two classmates, Vihan Jayaraman and Jerry Wang.

### Abstract

The main goal of our project was to construct a device that shoots projectiles with multiple degrees of freedom. We mounted a ping-pong ball launcher on a tiltable mount, giving it 360 degrees of coverage in aim. Using a wirelessly connected PS4 controller, we send commands to the Arduino’s serial monitor, which rotates and tilts the turret to aim and fire our ping-pong balls. 

### Technical Details

**Software**: Using AntiMicroX, we mapped the PS4 controls to keyboard commands. Afterwards, we used the serial monitor emulator PuTTY to ensure all keyboard commands were immediately sent to the Arduino. The Arduino then reads the keyboard commands from PuTTY and executes them.

**Hardware**: The entire system is powered using a 12V power supply. We designed a MOSFET circuit to act as a switch for the spindle motors and used the Arduino to control the Nema 17 stepper motors. 

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

We took heavy inspiration from an online [arduino lab](https://projecthub.arduino.cc/GordPayne/arduino-ping-pong-ball-cannon-abb8b3), with a design very similar in terms of mechanics. We enhanced the design further with CAD to make it 3-D printable.

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