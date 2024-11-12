---
layout: home
title: FPGA VGA Driver Projext
tags: fpga vga verilog
categories: demo
---

The aim of this project is to adapt a FPGA VGA Driver to display a graphic onto a 640x480 display. 
This will all be done through Verilog and demonstarted on the Basys3 development boards.

## **Template VGA Design**
### **Project Set-Up**
We set up the project in Verilog based on code given to us by our lecturer. The board being used is a Basys3 development board which is a member of the artix-7 family, below you can see an image of what the initial set up of the project looks like.
<img src="https://github.com/NaoiseOL/FPGAProject/blob/main/Project%20summary.png">
### **Template Code**
We were given some Template code to get us started on the project. This code included design sources for VGA Sync and a colour cycle source we can use to determine the patter that is outputted onto our screen from out basys3 board.
#### **VGA_Sync**
<img src="https://github.com/NaoiseOL/FPGAProject/blob/main/VGASync.png">
Above you can see the VGA Sync file is setting the parameters of the display we want the graphic from the Board to fit. It sets all general information in regards to our VGA display and its settings.

#### **Colour_Sync**
<img src="https://github.com/NaoiseOL/FPGAProject/blob/main/colourCycle.png">
Above we can see a logic state machine which is used to determine the pattern used in our template code. In this code we filter through a range of different colours that is outputter to our screen.

### **Simulation**




