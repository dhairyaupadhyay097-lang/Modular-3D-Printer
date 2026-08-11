# Modular 3D Printer
![image](https://cdn.hackclub.com/019ead2c-0446-70e4-b238-ad2acf197a35/image.png)
It's a custom-build, Modular 3DP for rapid prototyping and developing crazy projects. 200 × 200 × 200 mm build volume to print PETG and PLA parts. My main aim for this project is not just building this printer, but learning mechanics, integrating parts built in CAD, and minute configurations needed for next big projects.

## Overview

## Story and Motivation

I have been fascinated by Tony Stark and his approach to engineering since I was young. What interested me most was not simply the technology he used, but the idea of being able to imagine something and then build it in the real world.
As I started working on robotics, electronics, and CubeSat projects, I realized that rapid prototyping was the key. I often imagined custom part but having them seems easy and practical. so, I decided, instead of buying a commercial 3D printer, I'll build one myself. Time was a constrain for me as a student, so I decide to overcome that.
This is not just a printer; it's like skeleton of future projects. It will give shape to every single project I'll make. So, its just the starting of next complex projects and design I have planned. It's also the first one in HCB also so it's kind of special.

## Who Is This Project For?
This project is intended for:
- Students learning mechanics
- Beginners interested in building a 3D printer
- people interested in 3DP
- Robotics and electronics enthusiasts

## Goals
Main aim is to build a medium for me to make other projects' 3D body and prototypes and cutting these printing costs too. Thats for me but for others they may differ

## Features
- 200x200x200mm build volume
- Belt driven X and Y axis
- Lag screw (threaded rods) driven Z axis for better stability
- Marlin firmware
- Heated print bed
- Modular structure
- PLA and PETG printables
- All-metal hotend
- 0.4 mm nozzle
- low cost and beginner friendly prototype

## Specifications

| Specification | Value |
|---|---|
| Build volume | 200 × 200 × 200 mm |
| Nozzle diameter | 0.4 mm |
| Filament | PLA, PETG |
| Typical layer height | 0.1–0.3 mm |
| X-axis | Belt and pulley |
| Y-axis | Belt and pulley |
| Z-axis | Lead screw |
| Hotend | All-metal |
| Cooling | Fan-cooled hotend |
| Firmware | Marlin |
| Heated bed | Yes |
| Target bed temperature | 60 °C |
  
## How It Works
the printer uses three linear motion systems to place print head and build layer together.

### X Axis
This motion is controlled by stepper motor and timing belt with timing belt pulley to move the print head horizontally.
<img width="1325" height="520" alt="image" src="https://github.com/user-attachments/assets/261d5eeb-0470-4bbd-b3c5-1823f5b51378" />

### Y Axis
similar as the X axis one, just the change is that to move whole system and not just the print head, I've use 2 motors to move it back and forth.
<img width="1020" height="338" alt="image" src="https://github.com/user-attachments/assets/05a0af59-dfd0-4fd3-bce3-0f950affde4c" />

### Z Axis
To enhance the stability and due to gravity, I have used lead screws to drive the heatbed up and down.
<img width="308" height="477" alt="image" src="https://github.com/user-attachments/assets/6b95a98d-4d26-4387-b47c-d640a163ac66" />

**For the stability and accuracy i have used smooth rods in all the axis.

### Extruder and Hotend
Filament is fed into the hotend by the extruder motor. The hotend heats the filament until it reaches the required printing temperature, allowing the material to be deposited layer by layer.
<img width="359" height="466" alt="image" src="https://github.com/user-attachments/assets/00ea7f13-8660-4d72-a877-d08939370004" />


### Heated Bed
provides a controlled printing surface and improves first-layer adhesion for materials such as PLA and PETG.

## Electronics
- Arduino mega
- Ramps 1.4 shield
- Nema 17 Stepper motor
- A4988 motor controller
- endstops
- thermistors
- few wires and LEDs ofc
- Cooling fan for hotend
- E3D hotend

## Firmware
The printer uses Marlin firmware running on an Arduino Mega 2560 with a RAMPS 1.4 (shield) control board.
The firmware is configured specifically for this-

- Motion system
- Stepper motor drivers
- Build volume
- Endstops
- Extruder
- Hotend
- Heated bed
- Thermistors

I will upload complete firmware configuration in this repository so that the printer can be reproduced and configured by others.


## CAD and Mechanical Design
All custom CAD designs in this repository were created by me.
The CAD directory contains:

- Complete printer assembly
- Frame components
- Motor mounts
- Extruder components
- X, Y and Z-axis components
- Bed mounting components
- Custom brackets
- Other 3D-printed structural parts

Just get the name of file you need in the CAD section :)


## Bill of Materials
BOM is given above in its section


## Assembly and Printing
For assembly, check the Buildup page and Printing guide.

## Software
- CAD: for mechanical parts and body
- Slicer: Used to convert 3D models into G-code
- Marlin: Firmware used to control the printer's motors, heaters, fans, and sensors.
- Pronterface: Used to send G-code, control the printer, and test/calibrate its systems.

## Testing and Calibration
After assembly, the printer will be tested and calibrated in several stages.

- Mechanical Testing
- Motion Calibration
- Temperature Calibration
- Print Testing

For detail, check the testing page

## Project Photos
No mess here, photos of the build, assembly, and testing process are available in the Gallery
https://github.com/dhairyaupadhyay097-lang/Modular-3D-Printer/tree/main/Images

## Firmware Files
under development

## Future Improvements
- Adding a screen for manual control
- better structure
- better print speed
- fast modelling
- monitoring and filament run out detector
- spaghetti detector too :)

## Problems and Lessons Learned
till now faced tons of problems from CAD and electronic selection and also hope i face them more and more as it will help me to make a better 3DP, i'll update about'em.

## Safety
- Be aware of Hotend and heatbed as they may be hot
- take care of current
- also do not rush to build it
- keep children and untrained users away
- do not leave the printer unattended during testing.
- disconnect power before maintenance or modifications. 

