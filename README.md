# mulACS
 --- A dormitory Access Control System (ACS) with multiple authentication methods

### Video [![IMAGE ALT TEXT](http://img.youtube.com/vi/oCX-VuLmbKk/0.jpg)](http://www.youtube.com/watch?v=oCX-VuLmbKk)

### Video 2 --- Field Test


## Introduction
**mulACS** is a dormitory Access Control System (ACS) that supports two authentication methods --- ***Student Card*** & ***Android APP***.
It is a course project for *(ES004) Electronics System Design Based on Android System* (Summer 2015). 


This project focuses on the following troublesome scenarios. 
* Someone is knocking on the door while you are in bed with nobody else indoor. 
* The key to the door is lost somewhere or left in the dormitory.
* An old-fashion key is stuck in the hole when you urgently want the door open. 

Given that smartphones and student cards are frequently used on campus and less likely to lose or neglect, we provide a dual-mode dormitory ACS resolution utilizing RFID and Bluetooth.

### Mode 1 --- Student Card
Student cards are usually S50/S70 IC cards. Every card is given a unique U.I.D. when manufactured. 

Based on RFID, **mulACS** can read the cards and tell whether they are valid or not.
Once a valid student card is detected, the door will be opened by an Arduino-driven servo.

### Mode 2 --- Android APP
A specific Android APP is created for **mulACS** to realize 'One-button' authentication.

When the APP is initialized, the smartphone will automatically and transparently connect the microcontroller (Arduino) via Bluetooth with special PIN number. 
Once the user presses the "Open" button on the screen, a command will be sent.
The microcontroller will check the connected devices and response to the "OPEN" commands.


## Webpage

[http://eelab.sjtu.edu.cn/summer/2015/A06/index.html](http://eelab.sjtu.edu.cn/summer/2015/A06/index.html "mulACS Report Webpage (in Chinese)")

The link above points to the report webpage (in Chinese) with implementation details. 


## Contribution
Focus on Android Bluetooth implementation, RFID&LCD module test, code for Arduino (microcontroller), mechanical structure development, Demo video and report webpage.

Lead the development of the whole system.


## Details(selected)

[Figure 1 illustrates the connections among Arduino system modules](/path/to/img.jpg "The Connections among Arduino System Modules")
