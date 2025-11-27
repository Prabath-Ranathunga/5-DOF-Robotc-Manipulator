# 5-DOF Robotic Manipulator

This repository contains the research, design, and implementation of a compact 5-degree-of-freedom (DOF) robotic manipulator. The project focuses on the complete development lifecycle, from initial design and simulation to the physical implementation and control of the robotic arm, making it suitable for rapid prototyping, research, and light-duty material handling applications.

## Little bit about project:
The development of a 5-DOF robotic manipulator, designed for versatility and precision in a compact form factor. The project encompasses the mechanical design using 3D-printed components to keep the manufacturing cost of this as low as possible. The manipulator's performance is validated through extensive simulation and a physical prototype, demonstrating its capabilities in tasks such as pick-and-place operations and path following. The results establish it as a viable and accessible platform for academic research, educational purposes, and light-duty industrial automation.

## Key Specifications

| Specification      | Value                               |
| ------------------ | ----------------------------------- |
| **Degrees of Freedom** | 5                                   |
| **Reach**              | ~350mm                              |
| **Positional Accuracy**| ±2mm                                |
| **Frame Material**     | 3D Printed PLA/PETG                 |
| **Control System**     | Microcontroller-based               |

## Design
The design of the robot arm itself based on 5-axis movements, to have very high levels of movement and accuracy. So its have three rotary axis and 2 linear axis. The speciality about this robot from others was the whole robot rotate around the workspace, so whatever its working on stays still. The main idea was to keep everything compact. 

The base axis called `R_360-axis`  is the main axis that rotate around the main platform while carrying all other axis and it holds whole weight of the robot arm. To get a smoother movement and reduce the axis play a triple cycloidal disk gear system was used instead of dual 
cycloidal disk design. Crossed roller slewing bearings are used in this design to reduce any friction on output housing. `R-axis` is linear axis that can vary the radius of robot arm movements and that uses motor rotary movements and converted into linear movement by mean of a lead screw and nut. To grain accurate smooth movements with ability to accommodate heavy axial loads, linear guide rails ware used to drive this axis. `Z-Axis` is also a linear axis that same as the `R-axis` but in vertically. This design also used linear 
guide rails and lead screw setup to drive the joint. `J-Axis` joint don’t have too much load. so, these joint uses two cycloidal disks instead of three cycloidal disks that attached to eccentric shaft to drive the joint. To carry all radial loads, two ball bearings were used in each side of the output housing. This `I-Axis` joint work same as the `J-Axis` joint. In this design main housing back plate is used to mount this joint component to the `J-Axis` arm.

## Prototyping 
Most of the parts in the machine are done by 3D printing, considering the requirements such as strength, price and printerbility, PETG was a great choice. The hard part of printing or prototyping is the gear-drive parts, since those cycodial parts have tight tollarance had to pring over and over again to test best fit to archive zero play(or very close to) drive. Other than that its mostly fitting parts together with M3 nuts & bolts and bunch of heat inserts. 

## License
This publication is © 2022 [Prabath Ranathunga | ISSN 2961-502X].  
All rights reserved.  
No part of this work may be reproduced, distributed, or adapted without explicit written permission.