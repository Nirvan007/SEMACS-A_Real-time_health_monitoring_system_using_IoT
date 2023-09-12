Real time healthmonitoring band using Internet of Things <a name="TOP"></a>
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
* [SEMACS Application UI](#SEMACS-Application-UI)
* [References](#References)

## Introduction
A real-time health monitoring system (Health Band) that monitors health related parameters like Heart rate, SpO2, Body temperature, Room temperature, Sleep duration, Fall detection and Emergency call button. This device was intended to be used by elderly people and patients (non-serious) that live alone away from their family and hence, the name SEMACS - Smart Elderly Monitoring and Care System. With the help of IoT, the relatives or the family members of these individuals can keep a check on the person who is wearing it, and also be able to get a notification if there is any mishap, or emergency. This band can also be used by people who want use it as a regular health or fitness band inorder to check their health and performance in day-to-day life. 

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
* All heatlh related data is stored and forwarded to the application in real-time using a Real-Time Database (RTDB) with the help of Google Firebase.
* 1000 mAh lithium-ion battery that is rechargeable and gives a long battery backup.

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
* 802.11 n support (2.4 GHz ~ 2.5 GHz), up to 72.2 Mbps 
* USB-TTL based on CP2102 is included onboard, Enabling Plug n Play
* Onboard PCB Antenna

## Microcontroller Interfacing
* Used I2C protocol to interface the microcontroller to:
  1. MAX30102 Heart rate and Pulse Oximeter sensor for Heart rate and SpO2 monitoring.
  2. MPU6050 Gyroscope and Accelerometer for sleep detection and fall detection.
  3. 128x64 OLED Display for displaying all the measured parameters to the user.
* Used WiFi (2.4GHz) for Connectivity with the SEMACS Mobile Application.
* Interfaced the DS18B20 Digital temperature sensor to monitor the body temperature.
* Interfaced the DHT11 Temperature and Humidity sensor to monitor the room temperature and humidity.
* Push Button for switching screens on the OLED display and for sending an emergency call notification.

## Schematic
![image](https://user-images.githubusercontent.com/127144315/223844096-c96638e7-28e1-4cd9-b39b-7ca7b42ead74.png)

## Google Firebase (Back-end Real-Time Database)
#### Projects interface
![image](https://user-images.githubusercontent.com/127144315/223844498-3c206e85-dd1c-41f6-998f-936464151265.png)

#### SEMACS Project Overview
![image](https://user-images.githubusercontent.com/127144315/223844840-717feab1-2709-4f5d-92d9-6bd8a7ac7aec.png)

#### SEMACS Real-Time Database
![WhatsApp Image 2023-03-09 at 2 23 30 AM](https://user-images.githubusercontent.com/127144315/223847460-ce3c80cb-12b4-41f8-a68a-bc4bb17bbfea.jpeg)

#### Parameter Display
![WhatsApp Image 2023-03-09 at 2 23 30 AM (1)](https://user-images.githubusercontent.com/127144315/223847522-d2eddc7b-c720-4bbe-ab90-4611382727a1.jpeg)

## SEMACS Application UI
#### Main Dashboard
![WhatsApp Image 2023-03-09 at 1 21 38 AM](https://user-images.githubusercontent.com/127144315/223833541-a061c01b-c190-46f0-ba09-0a1ba1cc4de5.jpeg)

## References
 - [1] https://www.analog.com/en/products/max30102.html#product-overview
 - [2] https://ieeexplore.ieee.org/document/8540606
 - [3] https://lastminuteengineers.com/max30102-pulse-oximeter-heart-rate-sensor-arduino-tutorial/#:~:text=MAX30102%20Module%20Pinout,-The%20MAX30102%20module&text=You%20can%20connect%20it%20to,an%20interrupt%20for%20each%20pulse.
 - [4] https://ieeexplore.ieee.org/document/9153994
