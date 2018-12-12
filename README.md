# LIS3DH 3-Axis Accelerometer
## Created by: Anshul Sanan
## Humber Institute of Technology and Advanced Learning
## CENG 317 Instructor: Kristian Medri

## Table of Contents
1. [Introduction](#introduction)

2. [Parts Required and Budget](#Part-Required-and-Budget)

3. [Time Commitment](#time-commitment)

4. [Raspberry Pi Setup](#raspberry-pi-setup)

5. [Structure of my Project](structure-of-my-project)

6. [Assembling ](#assembling)

7. [Soldering ](#Soldering)

8. [Testing](#testing)

9. [Final Product](#final-product)

10. [Resources](#resources)



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

## Raspberry Pi Setup

![rpi3b](https://user-images.githubusercontent.com/42980862/49776194-078b5d00-fcc9-11e8-8d61-f96a17dfd31c.PNG)

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

![mfg_sen-13963_sml](https://user-images.githubusercontent.com/43185859/49842414-74662c00-fd89-11e8-8832-43866cd63316.jpg)

#### Step 1:
Plug the USB keyboard and mouse into the USB ports of the Raspberry Pi.
Plug the HDMI or video component cable into the monitor or TV set used.
Insert the Ethernet Cable from Raspberry Pi to one on your computer.

#### Step 2:
Turn on your monitor or TV set and make sure it is set to the proper input (e.g. HDMI 1 or HDMI 2) and also
connect the power supply to your Raspberry Pi .
A power indicator light will begin to glow, letting you know that you are connected,

#### Step 3:

## Structure of the Project

![49117469-c75ec000-f26e-11e8-89de-af591b191b37](https://user-images.githubusercontent.com/43185859/49842474-b5f6d700-fd89-11e8-9434-e78c4d0f42c8.PNG)


## Assembling 

### Pinout
![PinOut](https://user-images.githubusercontent.com/43185859/49836083-60adcc00-fd6f-11e8-8d52-28c39597ddc8.png)

* Connect 3.3V on the Raspberry Pi to VCC of the Sensor
* Connect GND on the Raspberry Pi to GND of the Sensor 
* Connect SCL(GPIO3) on the Raspberry Pi to SCL of the Sensor
* Connect SDA(GPIO2) on the Raspberry Pi to SCL of the Sensor
![whatsapp image 2018-12-11 at 8 37 01 pm](https://user-images.githubusercontent.com/43185859/49841188-9e691f80-fd84-11e8-8f8d-2ee5c1502a8d.jpeg)

### I2C Detection

Next, to ensure the LIS3DH has been connected properly for I2C communications, the following command should be entered in to the Pi's terminal: 
```
sudo i2cdetect -y 1

```
This will display a simple graphic listing each device connected to the I2C bus and it's corrisponding address. The address the LIS3DH uses is 0x19.

![I2C Reading](https://user-images.githubusercontent.com/43185859/48022115-4f3a2a00-e108-11e8-85be-6037c6ad8365.jpg)
## Soldering



Fritzing File:
https://github.com/anshulsanan/smart_wear/files/2621943/Accelerometer.zip

##### PCB Design:
![49475847-524b3780-f7e6-11e8-89f2-b46c55de2339](https://user-images.githubusercontent.com/43185859/49842577-15ed7d80-fd8a-11e8-967e-6661e784ba59.jpg)

 After designing the pcb I statred soldering it .
 This are the safety measures one should follow to do proper soldering to the pcb without any acciedent. 
 ### 5 Steps for Soldering:

1. Heat up your iron (600-700 degrees F or 315-370 degrees C)

![a](data:image/webp;base64,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)

2. Make sure connection are mechanically stable using helping hands to keep parts steady.

![b](https://user-images.githubusercontent.com/42980862/49781552-2b5a9d00-fce1-11e8-82dd-deca47e9e57e.PNG)

3. Clean iron that builds oxide layer, which inhibits heat transfer and solder adhesion using sponge wire.

![image](https://user-images.githubusercontent.com/42980862/49781575-43cab780-fce1-11e8-95ad-500c5b4705eb.png)

4. Apply heat and solder (soldering time sometimes varies)

![c](https://user-images.githubusercontent.com/42980862/49781732-dd926480-fce1-11e8-9c6f-daf2468aa2b8.PNG)

5. Inspect the join ( Smooth and shiny surface can be observed using a microscope)

Top:
![49110986-e6545680-f25c-11e8-8d6d-bffd694687bc](https://user-images.githubusercontent.com/43185859/49842849-218d7400-fd8b-11e8-9542-1fad94adba12.jpg)

Botton:
![49110987-e6545680-f25c-11e8-92ab-5fbddac78d77](https://user-images.githubusercontent.com/43185859/49842865-2baf7280-fd8b-11e8-9b1c-dfb00e3c5f6d.jpg)


## Testing
Compile and Build the following code to execute the sensor and get readings -:

[LIS3DH 3-Axis Accelerometer Python File](https://github.com/anshulsanan/smart_wear/files/2621855/LIS3DH.zip)


![Readings](https://user-images.githubusercontent.com/43185859/49110905-b311c780-f25c-11e8-9c8d-693c720bd9f8.jpg)

#

## Final Product
![Final Product](https://user-images.githubusercontent.com/43185859/49110782-662df100-f25c-11e8-8278-cf184d9ccf36.jpg)


#

## Resources

#
