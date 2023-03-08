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

## Microcontroller Interfacing
* Used I2C protocol to interface ESP32C3 Microcontroller to IP5328P Power Bank SoC
* Used BLE 5.0 for Connectivity with the SmartBank Mobile Application
* Interfaced DS18B20 Digital temperature sensor to monitor the Power Bank's battery temperature
* LED and Buzzer for the Find My Device Feature as an output device
* Push Button for Turning ON/OFF, Torch, and Connectivity

## SEMACS Application UI
#### Onboarding (Start-up) screen


#### Main Dashboard


## References
 - [1] 
 - [2] 
 - [3] 
