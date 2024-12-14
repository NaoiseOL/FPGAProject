---
layout: home
title: FPGA VGA Driver Projext
tags: fpga vga verilog
categories: demo
---

The aim of this project is to adapt a FPGA VGA(Video Graphics Array) Driver to display a graphic onto a 640x480 display. 
This will all be done through Verilog and demonstarted on the Basys3 development boards.

## **Template VGA Design**
### **Project Set-Up**
We set up the project in Verilog based on code given to us by our lecturer. The board being used is a Basys3 development board which is a member of the artix-7 family, below you can see an image of what the initial set up of the project looks like.
![Project summary](https://github.com/user-attachments/assets/80053d92-22cc-4332-a24d-b2eb74509bc7)
### **Template Code**
We were given some Template code to get us started on the project. This code included design sources for VGA Sync and a colour cycle source we can use to determine the patter that is outputted onto our screen from out basys3 board.

The VGA uses analog signals to transmit video data from a source to a display device. These signals consist of three key components: RGB (Red, Green, Blue) which correspond to the brightness of the three primary colours, the Vsync(vertical sync) which is the indicator for the next frame in a video, and the HSync(Horizontal sync) This indicates a new line of pixels in a video.
#### **VGA_Sync**
![VGASync](https://github.com/user-attachments/assets/1d7ea664-2032-4d15-9fd7-9608c0f6e39d)

Above you can see the VGA Sync file is setting the parameters of the display we want the graphic from the Board to fit. It sets all general information in regards to our VGA display and its settings.

#### **Colour_Sync**
![colourCycle](https://github.com/user-attachments/assets/c00f16b6-1a16-41d8-8651-000426fff71b)

Above we can see a logic state machine which is used to determine the pattern used in our template code. In this code we filter through a range of different colours that is outputter to our screen.

#### **Colour_Stripes**
![colourStripes](https://github.com/user-attachments/assets/b4000cd9-012b-4ad0-98eb-b9ca1ab89820)

Above is the original colourStripes code we were given to work off. The function of the code was creating stripes of different colours along the screen determined by columns and rows. Each column is one pixel across from left to right and each row is a pixel from top to bottom. The amount of rows is set when you are setting screen size within VGA_Sync 
## **MY VGA DESIGN**
For my design I decided to create a day/night cycle over a green landscape of a small wood or forest. It is very achievable, however also quite complex therefore I used to assistance of AI powered chatbots to help in developing the code and then in turn editing it to my own preferences. Primarily using CoPilot or Chatgpt when needed.

### **Code Adaptation**
Initially I started by setting out the dimensions for my image. Starting by determining the size of my green landscape vs my Sky to have the day/night cycle. I did this by setting all rows more than 350 as greenery and rows less than 350 as our sky.

### **Simulation**
![SimulationImg](https://github.com/user-attachments/assets/b07772b3-f98e-4385-a65c-eccdd5174bd9)

Above we can see our simulation of the template project which filter through the different colours, rows and columns based on the clock being used which allows us to see the patterns outputted onto the Screen when implemented onto the board.

### **Synthesis**
![Synthesis Schematic](https://github.com/user-attachments/assets/258439bd-3c08-40de-aa11-f1ae85fe8e17)

Above is the Schematic of the project code at the synthesis stage.







