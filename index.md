# Week13 (Nov 27)

**Presentation Week:**

[LIS3DH.pptx](https://github.com/anshulsanan/smart_wear/files/2646064/LIS3DH.pptx)

# Week12 (Nov 20)

**Enclosure-**

**Progress Report-**
The acrylic case printed for my enclosure was a little tight and couldn't house some of the I/O ports so I reprinted my acrylic case and attathed my RPi in it.

![img_20181127_154826](https://user-images.githubusercontent.com/43185859/49110781-662df100-f25c-11e8-923a-a5a6c2d52e57.jpg)
![img_20181127_154831](https://user-images.githubusercontent.com/43185859/49110782-662df100-f25c-11e8-8278-cf184d9ccf36.jpg)
![img_20181127_154811](https://user-images.githubusercontent.com/43185859/49110784-662df100-f25c-11e8-840a-9c4cca669a2f.jpg)
![img_20181127_154815](https://user-images.githubusercontent.com/43185859/49110785-662df100-f25c-11e8-9686-bdb6de588d4d.jpg)
![img_20181127_154822](https://user-images.githubusercontent.com/43185859/49110787-662df100-f25c-11e8-9b44-da08c71257b2.jpg)
![img_20181127_154824](https://user-images.githubusercontent.com/43185859/49110788-662df100-f25c-11e8-86cd-19be71ad2ddc.jpg)

**CorelDraw File :**

[Anshul_CorelFile.zip](https://github.com/anshulsanan/smart_wear/files/2621935/Anshul_CorelFile.zip)

![capture](https://user-images.githubusercontent.com/43185859/49113049-78ab2900-f262-11e8-9450-ad23d13df45b.PNG)


# Week11 (Nov 13)

**Power Up and Readings:**

I faced many obstacles with the code and my sensor as I bought a sparkfun sensor which is compatible mostly with arduino microcontroller . So , I have to take it to next level and download some plug-ins and libraries which took some time but finally worked at last.

**Progress Report-**

I chose a sparkfun sensor and because of its inavailibility of python files, I had to make changes to the files of same sensor provided by Adafruit which worked successfully for me.The piduino library support ,toolchain and StackOverflow helped me to get the readings.

![whatsapp image 2018-11-28 at 7 43 48 pm](https://user-images.githubusercontent.com/43185859/49191801-20e5ee00-f346-11e8-9abf-355269255ad0.jpeg)

![lis3dh](https://user-images.githubusercontent.com/43185859/49110905-b311c780-f25c-11e8-9c8d-693c720bd9f8.jpg)

**Files Used:**

[LIS3DH.zip](https://github.com/anshulsanan/smart_wear/files/2621855/LIS3DH.zip)


# Week10 (Nov 6)

**PCB Printing-**

**Progress Report-**

During the soldering process, I made many shorts but with the help of Vlad, I removed that shorts.

![img_20181127_125248](https://user-images.githubusercontent.com/43185859/49110983-e6545680-f25c-11e8-90ee-d589fa343b9c.jpg)
![img_20181127_125306](https://user-images.githubusercontent.com/43185859/49110984-e6545680-f25c-11e8-8166-9b20dbacd200.jpg)
![img_20181127_125310](https://user-images.githubusercontent.com/43185859/49110985-e6545680-f25c-11e8-9ffc-416bb18ab27e.jpg)
![img_20181127_125209](https://user-images.githubusercontent.com/43185859/49110986-e6545680-f25c-11e8-8d6d-bffd694687bc.jpg)
![img_20181127_125213](https://user-images.githubusercontent.com/43185859/49110987-e6545680-f25c-11e8-92ab-5fbddac78d77.jpg)
![img_20181127_125220](https://user-images.githubusercontent.com/43185859/49110988-e6545680-f25c-11e8-9388-539b7eb1c4ce.jpg)


# Week9 (Oct 30)

**PCB Design -**

**Progress Report-**
I sent my gerbert file to Vlad and it took many attempts to print it due to some minor defects and because other students accidentally taking PCBs thinking its theirs.Also, many times the Prototype Lab didn't receive my email a few times.

**Gerbert File:**

[Accelerometer.zip](https://github.com/anshulsanan/smart_wear/files/2621943/Accelerometer.zip)


![whatsapp image 2018-11-05 at 2 25 06 pm 1](https://user-images.githubusercontent.com/43185859/48021714-43019d00-e107-11e8-8637-334db220a56a.jpeg)

![whatsapp image 2018-11-05 at 2 25 06 pm](https://user-images.githubusercontent.com/43185859/48021784-6d535a80-e107-11e8-9ba3-1162ebdee2af.jpeg)

![33c6e3d3-62be-4958-8fb5-e9c726f1eecd](https://user-images.githubusercontent.com/43185859/48021885-b3102300-e107-11e8-80c8-58d16e0771ab.jpg)


# Week8 (Oct 23)

**Connection and i2c detection-**

I connected the 3V pin to the Positive Power Rails(+) and Ground to the Negative Power Rails(-).
I connected the SCL pin of the Pi to SCL of the sensor and SDA pin of Pi to SDA on the sensor.
After starting my Pi,I used the command "i2cdetect -y 1" in terminal and I got my address to be 0x19.

**Progress Report-**

There was no problem in getting the address of the i2c bus as from the first time,the connections were right.

![i2c_bb](https://user-images.githubusercontent.com/43185859/48022114-4d706680-e108-11e8-8b9d-90162020e282.jpg)

![img_20181023_165739](https://user-images.githubusercontent.com/43185859/48022115-4f3a2a00-e108-11e8-85be-6037c6ad8365.jpg)


# Week7 (Oct 16)
**Aquisition-**

The Parts I Recieved in the kit included -
1 Raspberry Pi 3b+

![770a5842-1612x1080](https://user-images.githubusercontent.com/43185859/49117549-14db2d00-f26f-11e8-916a-be875860f58f.jpg)

1 LIS3DH 3-Axis Accelerometer

![lis3dh](https://user-images.githubusercontent.com/43185859/49117559-1dcbfe80-f26f-11e8-9312-64969a31ff77.jpg)


# Week6 (Oct 9)

**UML Diagram-**

I worked with a first year student to make pseudo code for the project and we completed it on time.

Link to Pseudo Code-

[Pseudo Code.pdf](https://github.com/anshulsanan/smart_wear/files/2622681/Pseudo.Code.pdf)

![capture](https://user-images.githubusercontent.com/43185859/49117469-c75ec000-f26e-11e8-89de-af591b191b37.PNG)


# Week5 (Oct 2)
**Invoice-**

The invoice includes the raspberry pi and my lis3dh sensor ordered by me. 

![anshul](https://user-images.githubusercontent.com/43185859/46379071-b5e0a980-c66b-11e8-9678-66c474e7509c.PNG)


# Week4 (Sep 25)

**Budget:**

My Budget for this project was upto $200-$300 and while researching for parts , it came all under my budget.

[Budget.docx](https://github.com/anshulsanan/smart_wear/files/2550329/Budget.docx)


![capture](https://user-images.githubusercontent.com/43185859/48022365-f4ed9900-e108-11e8-9cdd-c8d549768096.PNG)


# Week3 (Sep 18)
**Schedule-**

I made a schedule for the project for which i posted the link below.

[Schedule.zip](https://github.com/anshulsanan/smart_wear/files/2622669/Schedule.zip)

![47387249-c1f4df80-d6dc-11e8-9725-7fe4e579356e](https://user-images.githubusercontent.com/43185859/48022671-c6bc8900-e109-11e8-933f-ec6e5755b92f.png)

# Week2 (Sep 11)
**Proposal-**

I made a proposal for my project for which i posted the link below.

(https://github.com/anshulsanan/smart_wear/files/2622662/ProposalContentStudent.xlsx)

![capture1](https://user-images.githubusercontent.com/43185859/48022555-75ac9500-e109-11e8-8790-4d3f4d5bbddd.PNG)

# Week1 (Sep 4)
