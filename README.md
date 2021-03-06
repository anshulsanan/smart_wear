# LIS3DH 3-Axis Accelerometer
## Created by: Anshul Sanan
## Humber Institute of Technology and Advanced Learning
## CENG 317 Instructor: Kristian Medri

## Table of Contents
* [Introduction](#introduction)

* [Parts Required and Budget](#Part-Required-and-Budget)

* [Time Commitment](#time-commitment)

* [Raspberry Pi Setup](#raspberry-pi-setup)

* [Structure of my Project](structure-of-my-project)

* [Assembling ](#assembling)

* [Soldering ](#Soldering)

* [Enclosure](#Enclosure)

* [Testing](#testing)

* [Production-Testing](#Production-testing)

* [Final Product](#final-product)


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
Follow all the procedure accordingly and complete the setup . Enable SSH , I2C and VNC in system configurations in the UI of PI.

### You have successfully completed the setup!!

![raspberry-pi-booting](https://user-images.githubusercontent.com/43185859/49844760-328db380-fd92-11e8-8ac8-bd6f4d5c2cdd.jpg)


#

## Structure of the Project

![49117469-c75ec000-f26e-11e8-89de-af591b191b37](https://user-images.githubusercontent.com/43185859/49842474-b5f6d700-fd89-11e8-9434-e78c4d0f42c8.PNG)

#

## Assembling 

### Pinout
![PinOut](https://user-images.githubusercontent.com/43185859/49836083-60adcc00-fd6f-11e8-8d52-28c39597ddc8.png)

* Connect 3.3V on the Raspberry Pi to VCC of the Sensor
* Connect GND on the Raspberry Pi to GND of the Sensor 
* Connect SCL(GPIO3) on the Raspberry Pi to SCL of the Sensor
* Connect SDA(GPIO2) on the Raspberry Pi to SCL of the Sensor
![Connection](https://user-images.githubusercontent.com/43185859/49841188-9e691f80-fd84-11e8-8f8d-2ee5c1502a8d.jpeg)

### I2C Detection

Next, to ensure the LIS3DH has been connected properly for I2C communications, the following command should be entered in to the Pi's terminal: 
```
sudo i2cdetect -y 1

```
This will display a simple graphic listing each device connected to the I2C bus and it's corrisponding address. The address the LIS3DH uses is 0x19.

![I2C Reading](https://user-images.githubusercontent.com/43185859/48022115-4f3a2a00-e108-11e8-85be-6037c6ad8365.jpg)

I made my PCB using the help of Prototype Lab at Humber College . But if you download the following fritzing file , you will be able to make the same PCB used by me as the Fritzing is an industry standard software and can be printed out wherever at a local PCB Print Shop or Online.

### [Fritzing File](https://github.com/anshulsanan/smart_wear/files/2621943/Accelerometer.zip)

##### PCB Design:
![49475847-524b3780-f7e6-11e8-89f2-b46c55de2339](https://user-images.githubusercontent.com/43185859/49842577-15ed7d80-fd8a-11e8-967e-6661e784ba59.jpg)
#
## Soldering

 After designing the pcb I started soldering it .
 This are the safety measures one should follow to do proper soldering to the pcb without any accident. 
 ### 5 Steps for Soldering:

### 1. Heat up your iron (600-700 degrees F or 315-370 degrees C)

![Heat-Iron](https://user-images.githubusercontent.com/43185859/49843840-85656c00-fd8e-11e8-9c45-8e4c7517fe41.jpeg)

### 2. Make sure connection are mechanically stable using helping hands to keep parts steady.

![b](https://user-images.githubusercontent.com/42980862/49781552-2b5a9d00-fce1-11e8-82dd-deca47e9e57e.PNG)

### 3. Clean iron that builds oxide layer, which inhibits heat transfer and solder adhesion using sponge wire.

![images](https://user-images.githubusercontent.com/43185859/49843906-d5dcc980-fd8e-11e8-8bf2-ee21a8c25a8f.jpeg)


### 4. Apply heat and solder (soldering time sometimes varies)

![c](https://user-images.githubusercontent.com/42980862/49781732-dd926480-fce1-11e8-9c6f-daf2468aa2b8.PNG)

### 5. Inspect the join ( Smooth and shiny surface can be observed using a microscope)

### Top View:

![49110986-e6545680-f25c-11e8-8d6d-bffd694687bc](https://user-images.githubusercontent.com/43185859/49842849-218d7400-fd8b-11e8-9542-1fad94adba12.jpg)

### Bottom View:

![49110987-e6545680-f25c-11e8-92ab-5fbddac78d77](https://user-images.githubusercontent.com/43185859/49842865-2baf7280-fd8b-11e8-9b1c-dfb00e3c5f6d.jpg)

#

## Testing
Compile and Build the following code to execute the sensor and get readings -:
I used this Python File for the Sensor-: 

[LIS3DH 3-Axis Accelerometer Python File](https://github.com/anshulsanan/smart_wear/files/2621855/LIS3DH.zip)


#### * In the Terminal , Go to your folder where LIS3DH.py exists.
#### * Enter ```python3 LIS3DH.py``` command and compile it.
#### * Extract all the libraries from the file : [Piduino](https://github.com/anshulsanan/smart_wear/files/2670392/piduino.zip)
#### * Copy and Paste all the Libraries in the "lib" folder
#### * Execute the compiled code by typing ```./LIS3DH``` .

#### You will get the following readings
# ![Readings](https://user-images.githubusercontent.com/43185859/49110905-b311c780-f25c-11e8-9c8d-693c720bd9f8.jpg)

# ![Code](https://user-images.githubusercontent.com/43185859/49845593-4e468900-fd95-11e8-8c27-8f3014d82888.png)

#

# Enclosure
I made my Enclosure using the help of Prototype Lab at Humber College . But if you download the following corel draw file , you will be able to make the same corel draw case used by me as the corel draw file is an industry standard and can be printed out wherever a 3D Printer is availible.

[Corel Draw File](https://github.com/anshulsanan/smart_wear/files/2670327/Anshul_CorelFile.zip)

![Enclosure](https://user-images.githubusercontent.com/43185859/49844967-d37c6e80-fd92-11e8-8ae6-85376e5acf01.jpg)

![Enclosure](https://user-images.githubusercontent.com/43185859/49844969-d4150500-fd92-11e8-8d45-bd95c4c54e42.PNG)

# Production-Testing

For the Production-testing One has no more need to solder it manually. THE whole Soldering job of the Project can be made automated.
Also the testing of the sensor can be made automated by moving the sensor to make the axis of the sensor to change.


#

## Final Product
![Final Product](https://user-images.githubusercontent.com/43185859/49110782-662df100-f25c-11e8-8278-cf184d9ccf36.jpg)


