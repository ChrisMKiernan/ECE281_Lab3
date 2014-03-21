# Lab 3

All files submitted are considered late by normal deadlines, but with permission from Capt Silva due to a week-long trip on SCA, the files are submitted late. 

## Prelab

The schematic for the prelab is below. The buttons and switches are left open for now, we'll use those later when we create the actual controller.

![alt text](https://raw.githubusercontent.com/ChrisMKiernan/ECE281_Lab3/master/Prelab_Schematic.jpg "Prelab schematic of the top Nexys 2 module")

## Lab

The next thing to do was to code and implement the lab. The first step was to add the Moore and Mealy machines as components in the program. After that, I could instantiate the components into the program. I put the Moore and Mealy component instantiations after the clock divider component (so that the respective machines could use the slower clock speeds) but before the nibble assignments (so that the outputs of the components could be input into the nibble assignments). This isn't where it was explicitly commented to modify the code, but it was the only place that seemed logical, given the shell's original state of the hanging inputs to the nibble components. 

When I submitted the Mealy controller portion of CE3, I clearly did not have a good understanding of what a Mealy machine looks like in VHDL. After further consideration, I started fresh with the Mealy machine from the original CE3 shell. From there I used code from the Moore machine and modified the output assignments to create a new Mealy machine. This new machine is what was used in the Nexys top architecture. 

## Functionality
Basic functionality was done via a video and uploaded to YouTube on the following link
https://www.youtube.com/watch?v=ufZD2MK20dw 
