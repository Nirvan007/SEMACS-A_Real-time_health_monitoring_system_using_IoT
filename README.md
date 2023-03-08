Real-time-health-monitoring-system-using-Internet-of-Things <a name="TOP"></a>
===================

## Table of Contents
* [Introduction](#Introduction)
* [Features](#Features)
* [Tools Used](#Tools-Used)
  * [EasyEDA](#EasyEDA)
  * [Arduino IDE](#Arduino-IDE)
  * [Fritzing](#Fritzing)
  * [Figma](#Figma)
  * [Flutter](#Flutter)
  * [Google Firebase](#Google-Firebase)
* [Hardware Components Used](#Hardware-Components-Used)
* [Microcontroller Specifications](#Microcontroller-Specifications)
* [Microcontroller Interfacing](#Microcontroller-Interfacing)
* [Schematic](#Schematic)
* [PCB](#PCB)
* [SEMACS Application UI](#SmartBank-Connect-Application-UI-Flow)
* [References](#References)

## Introduction
A real-time health monitoring system (Health Band) that monitors health related parameters like Heart rate, SpO2, Body temperature, Room temperature, Sleep duration, Fall detection and Emergency call button.

## Features
The SEMACS Health Band is equipped with the following features:
* Heart Rate monitoring
* SpO2 monitoring
* Body Temperature monitoring
* Room Temperature monitoring
* Room Humidity monitoring
* Sleep duration and sleepcycle monitoring 
* Fever or high body temperature detection
* Fall detection alarm and notification
* Emergency call button


## Unique Features
* Works on the Internet of Things, and hence health parameters of the user can be monitored from anywhere in the world with the help of an Internet connection.
* Parameter monitoring using SEMACS Mobile App
* 

## Tools Used
#### EasyEDA
EasyEDA is a web-based EDA tool suite that enables hardware engineers to design, simulate, share publicly and privately and discuss schematics, simulations and printed circuit boards.
* For more details refer: <https://easyeda.com/>

#### Arduino IDE 
Arduino Integrated Development Environment or Arduino Software (IDE) contains a text editor for writing code, a message area, a text console, a toolbar with buttons for common functions and a series of menus. It connects to the Arduino hardware to upload programs and communicate with them. 
* For more details refer: <https://www.arduino.cc/en/software>

#### Fritzing
Fritzing is an open-source hardware initiative that makes electronics accessible as a creative material for anyone. We offer a software tool, a community website and services in the spirit of Processing and Arduino, fostering a creative ecosystem that allows users to document their prototypes, share them with others, teach electronics in a classroom, and layout and manufacture professional PCBs. 
* For more details refer: <https://fritzing.org/>

#### Figma
Figma is a powerful web-based design tool that helps you create anything, websites, applications, logos, and much more. It is a vector graphics editor and prototyping tool that is often used for UI design.
* For more details refer: https://www.figma.com/

#### Flutter
Flutter is a mobile app development platform created by Google. It allows developers to create web, desktop, and cross-platform apps that run on Android and iOS devices. Flutter uses a reactive programming language called Dart, making development faster and easier than traditional methods. Flutter is an open source framework by Google for building beautiful, natively compiled, multi-platform applications from a single codebase.
* For more details refer: https://flutter.dev/

#### Google Firebase
Google Firebase is a Google-backed application development software that enables developers to develop iOS, Android and Web apps. Firebase provides tools for tracking analytics, reporting and fixing app crashes, creating marketing and product experiment. The Firebase Realtime Database is a cloud-hosted NoSQL database that lets you store and sync data between your users in realtime.
* For more details refer: <https://firebase.google.com/>

## Hardware Components Used

1. Nodemcu ESP8266 microcontroller
2. MAX30102 Heart rate and SpO2 sensor
3. DS18B20 Digital temperature sensor
4. MPU6050 Gyroscope and Accelerometer
5. I2C 128x64 OLED Display
6. Push Buttons

## Microcontroller Specifications
Espressif System's ESP8266 microcontroller has the following specifications:
* Tensilica 32-bit RISC CPU Xtensa LX106
* Operating Voltage: 3.3V
* Input Voltage: 7-12V
* Digital I/O Pins: 16
* Analog Input Pins (ADC): 1
* Peripherals Interfaces: 1 - UART, 1 - SPI, and 1 - I2C
* Flash Memory: 4 MB, SRAM: 64KB
* Clock Speed: 80 MHz
* USB-TTL based on CP2102 is included onboard, Enabling Plug n Play
* Onboard PCB Antenna

## Power Bank SoC Specifications
* Injoinic Technology IP5328P with Fully Integrated Bi directional PD3.0 and Fast Charge Power Bank SOC
* QFN-48 Package
* Support 5V, 9V, 12V voltage input/output
* Integrated USB Power Delivery (PD2.0/PD2.0) protocol
* Up to 5.0A charging current at battery port
* Adaptive charging current adjustment
* Discharge: 5V/3.1A (15W) 9V/2.0A (18W) 12V/1.5A (18W)
* I2C interface for flexible and low cost customized solution
* Single inductor for charging and discharging
* Output overcurrent, overvoltage and short circuit protection
* Battery overcharge, over discharge and overcurrent protection
* Over temperature protection
* Battery NTC protection

## SoC Pin Definition
![image](https://user-images.githubusercontent.com/127144315/223557740-36cd38b4-8c98-4057-8497-7916965bfec5.png)

## SoC I2C Connection
![image](https://user-images.githubusercontent.com/127144315/223559000-46c6d3b1-e2b1-4314-a11c-d28ab26bb6c2.png)

## SoC Application Component List
![image](https://user-images.githubusercontent.com/127144315/223559292-1a4c5e33-c9f5-49dd-859c-daf2097a57c7.png)

## Reference SoC Application Circuit Diagram
![SoC Reference Circuit](https://user-images.githubusercontent.com/127144315/223557157-5dd1aef8-1442-42fd-9f8d-2e75b665941f.png)

## SmartBank Charging Module
#### Schematic
![Schematic_SmartBank V2 0_2023-03-08](https://user-images.githubusercontent.com/127144315/223560833-468495cc-5802-4742-908d-133820ef0a78.png)

#### PCB
Top Layer

![image](https://user-images.githubusercontent.com/127144315/223562499-f002172f-948f-4635-8494-f3c16681e8b9.png)

![image](https://user-images.githubusercontent.com/127144315/223562064-7aebca20-e865-46a4-b882-e0b92bd076da.png)

Bottom Layer

![image](https://user-images.githubusercontent.com/127144315/223562559-14fdf376-e826-458a-b7b0-674ca9e3361d.png)

![image](https://user-images.githubusercontent.com/127144315/223561978-77fc8a1d-ea9c-48ac-8302-9f5ba9f3dc8b.png)

#### 3D PCB Model
![image](https://user-images.githubusercontent.com/127144315/223563612-a5669cda-3361-4dfd-ac4c-55b85a82aaa7.png)
![image](https://user-images.githubusercontent.com/127144315/223563678-b7caccbc-5913-4156-8b43-8a8badca0208.png)
![image](https://user-images.githubusercontent.com/127144315/223563867-22ac1ca5-fe47-4f34-ab56-8b9cfc9a6b94.png)
![image](https://user-images.githubusercontent.com/127144315/223563956-5cb6a7f8-9836-47d8-9def-073787bb7be8.png)

#### 3D Case Prototype Model
![CASE_V1](https://user-images.githubusercontent.com/127144315/223565589-ad6fab32-bca8-4f64-9298-f44475089ee4.png)

#### Fabricated PCB
![image](https://user-images.githubusercontent.com/127144315/223567838-76239e7f-ab74-4ea7-9fbd-33b273ab107b.png)
![image](https://user-images.githubusercontent.com/127144315/223567942-972300dd-691a-43cc-b769-739083b83d3f.png)

## Microcontroller Interfacing
* Used I2C protocol to interface ESP32C3 Microcontroller to IP5328P Power Bank SoC
* Used BLE 5.0 for Connectivity with the SmartBank Mobile Application
* Interfaced DS18B20 Digital temperature sensor to monitor the Power Bank's battery temperature
* LED and Buzzer for the Find My Device Feature as an output device
* Push Button for Turning ON/OFF, Torch, and Connectivity

## SmartBank Connect Application UI Flow
#### Onboarding (Start-up) screen
  ![image](https://user-images.githubusercontent.com/127144315/223569701-08bf7130-c0d9-4498-b507-af49af3a757e.png)

#### Search and Scan for devices
![image](https://user-images.githubusercontent.com/127144315/223569824-7ac3801d-94c6-4396-82cc-a1c5ce58d470.png)

#### Scan Fail/Error Connecting to device

![image](https://user-images.githubusercontent.com/127144315/223570078-9febf7a9-cc0c-4982-aec5-595f18282880.png)

#### Main Dashboard
![image](https://user-images.githubusercontent.com/127144315/223570145-b830e62d-bf16-46ae-a51e-5ef9e7b46c58.png)

#### Dashboard and Find My Device
![image](https://user-images.githubusercontent.com/127144315/223570180-042728c7-9de8-4bcd-9562-d5047397ecb2.png)

#### Settings, Connected Devices and Notification
![image](https://user-images.githubusercontent.com/127144315/223570371-b78765a1-8d30-4d6c-ba72-27583ee36ffc.png)

#### Usage History
![IMG-20220523-WA0009](https://user-images.githubusercontent.com/127144315/223571704-e967b5e7-0977-4336-8e10-0d493433b5e4.jpg)

#### Data Reset/Accessibilty Functions and T&C
![image](https://user-images.githubusercontent.com/127144315/223570588-7ff5fe9d-addc-4232-a1ac-8625e992a580.png)

## References
 - [1] http://www.injoinic.com/?lang=en-us
 - [2] https://www.mouser.in/
 - [3] https://www.lcsc.com/

## Acknowledgement
#### Project Mentors
1. Dr. Manoj Sankhe, BTI EXTC In-charge, MPSTME Mumbai Campus
2. Vishram Bapat, Founder, Databyte Services and Systems, http://databyteservices.com/

#### Guidance
* Ajit Bapat, CEO, Dataserve Pvt. Ltd., https://www.rightocare.com/ 
