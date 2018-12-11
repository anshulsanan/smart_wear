# LIS3DH 3-Axis Accelerometer
## Created by: Anshul Sanan
## Humber Institute of Technology and Advanced Learning
## CENG 317 Instructor: Kristian Medri

## Table of Contents
1. [Introduction](#introduction)

2. [Parts Required and Budget](#parts)

3. [Time Commitment](#time-commitment)

4. [Raspberry Pi Setup](#raspberry-pi-setup)

5. [Structure of my Project](structure-of-my-project)

6. [Assembling and Soldering](#assembling-and-soldering)

7. [Testing](#testing)

8. [Final Product](#final-product)

9. [Resources](#resources)



#

## Introduction

LIS3DH is an ultra low-power high performance three axis linear accelerometer belonging to the "nano" family, with digital I2C/SPI serial interface standard output.
The device features ultra low-power operational modes that allow advanced power saving and smart embedded functions.

#

## Part Required and Budget

The Parts involved includes-:

* [Raspberry Pi 3B+ Kit](https://www.amazon.ca/CanaKit-Raspberry-Complete-Starter-Kit/dp/B01CCF6V3A/ref=sr_1_5?s=pc&ie=UTF8&qid=1516324581&sr=1-5&keywords=Raspberry+Pi+3) - CAD$123.05
###
#### Specifications-:
* Quad core 64-bit processor clocked at 1.4GHz
* 1GB LPDDR2 SRAM
* Dual-band 2.4GHz and 5GHz wireless LAN
* Bluetooth 4.2 / BLE
* Higher speed ethernet up to 300Mbps
* Power-over-Ethernet capability (via a separate PoE HAT)

###
* [LIS3DH 3-Axis Accelerometer](https://www.sparkfun.com/products/13963) - CAD$21.20

#### Specifications:-
* Wide supply voltage, 1.71 V to 3.6 V
* Independent IO supply (1.8 V) and supply voltage compatible
* Ultra-low-power mode consumption down to 2 μA
* ±2g/±4g/±8g/±16g dynamically selectable full scale
* I2C/SPI digital output interface
* 16-bit data output
* 2 independent programmable interrupt generators for free-fall and motion detection
* 6D/4D orientation detection
* Free-fall detection
* Motion detection
* Embedded temperature sensor
* Embedded self-test
* Embedded 32 levels of 16-bit data output FIFO
* 10000 g high shock survivability
* ECOPACK®, RoHS and “Green” compliant 

#### Additional Parts

* Soldering Iron

* [Parts Kit(Cables)](https://www.circuitspecialists.com/circuits-basic-electronics-parts-kit.html)

* [Wire Strippers](https://www.circuitspecialists.com/heavy-duty-wire-strippers.html)

#### Optional

* Case (Can be Acrylic or Metal)

* PCB

* BreadBoard (Prototype)

#

## Time Commitment

The Project was made in the time frame of 15 weeks involving troubleshooting of many hardware components and software applications.
This project can be made in less than 3 weeks if the creator is experienced and parts are easily accessible to them.

![Image of Schedule](https://user-images.githubusercontent.com/43185859/49835353-e9773880-fd6c-11e8-879f-81fe9c096283.png)

#

## Raspberry Pi Setup

#

#### Operating System Setup

#### Step 1: 
When you're setting up the microSD card, you may need to use a microSD adapter. To begin setting this up, just slot the microSD card into the back of the microSD card adapter. To install the operating system on the microSD card, you'll need to use either an SD card reader/writer or you'll have a slot on your laptop for an SD card. In this instance, you take the SD card adapter and slot it into the reader. Then plug that reader into the computer and install the OS onto the microSD card.

#### Step 2:
Go to [Raspberry Operating System](https://www.raspberrypi.org/downloads/). 
You can either download NOOBS or RASPBIAN.Click your download of choice and wait for the download to complete.I will assume that RASPBIAN is downloaded.

#### Step 3:
Download [Win32 Disk Imager](https://sourceforge.net/projects/win32diskimager/) and install it on your computer.

#### Step 4:
Once you've downloaded the Raspberry Pi operating system, go to your Downloads folder and right click on that file, and click on 'Extract'  using [WinRaR](https://www.rarlab.com/download.htm).

After some time, you should have a folder with the same name appear next to the file. If you look inside, you can see the image file for the Raspberry Pi operating system. You'll now need to copy that over to the microSD card.

#### Step 5:
To copy your operating system image for the Raspberry Pi over to the microSD card, take your SD card reader from earlier, and plug it into a USB port on the computer. Alternatively, you can place the SD card into a card reader in your laptop.

Next, you'll need to copy the image for the operating system for the Raspberry Pi over to the microSD card. Open up Win 32 Disk Imager that you installed earlier, and you will see a window. Click on the blue folder icon, and find the image for the Raspbian Stretch operating system and then click 'Open'. Next, you need to pick the Device, by selecting the letter corresponding to the SD card reader. You'll see this letter appear inside Windows File Explorer when you plug the SD card reader in. Once that's selected then click 'Write'. Then wait some time, while the operating system is copied over to the SD card.

#### Step 6:
Once the operating system is installed on the SD card, take your board, turn it over. On the underside, you'll see a slot at the rear, which is where the microSD card needs to go. Take the microSD card, then insert it into the slot, gently, until it's firmly sitting inside.

##

#### PowerUp 

#### Step 1:
Plug the USB keyboard and mouse into the USB ports of the Raspberry Pi.
Plug the HDMI or video component cable into the monitor or TV set used.
Insert the Ethernet Cable from Raspberry Pi to one on your computer.

#### Step 2:
Turn on your monitor or TV set and make sure it is set to the proper input (e.g. HDMI 1 or HDMI 2) and also
connect the power supply to your Raspberry Pi .
A power indicator light will begin to glow, letting you know that you are connected,

#### Step 3:

#

## Structure of the Project

#

## Assembling and Soldering

#

## Testing
Compile and Build the following code to execute the sensor and get readings -:
[LIS3DH 3-Axis Accelerometer Python File]()

#

## Final Product

#

## Resources

#
