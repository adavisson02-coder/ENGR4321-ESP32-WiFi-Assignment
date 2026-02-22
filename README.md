<p align="center">

## ESP32 IoT Temperature & Humidity Monitoring System
</p> <p align="center">


</p> <p align="center"> <img src="https://img.shields.io/badge/Microcontroller-ESP32-blue?style=for-the-badge"> <img src="https://img.shields.io/badge/Sensor-DHT22-green?style=for-the-badge"> <img src="https://img.shields.io/badge/Cloud-Adafruit_IO-orange?style=for-the-badge"> <img src="https://img.shields.io/badge/Simulation-Wokwi-red?style=for-the-badge"> </p>

## Overview

This project implements a cloud-connected environmental monitoring system using the ESP32 microcontroller and a DHT22 temperature and humidity sensor. The ESP32 connects to a wireless network and publishes real-time sensor data to the Adafruit IO cloud platform using the MQTT protocol. This enables remote monitoring, data logging, and dashboard visualization — demonstrating a complete Internet of Things (IoT) system. This project was developed as part of ENGR 4321 – Microcontrollers & Embedded Systems at the University of the Incarnate Word.

## Live Simulation

Wokwi Project Link:

[https://wokwi.com/projects/456615498165739521](https://wokwi.com/projects/456615498165739521)

## System Preview
<p align="center"> <img src="https://github.com/user-attachments/assets/84d717b6-bc0e-45e2-bbf4-c03fe06dfdfc" width="450"> </p>
System Architecture
DHT22 Sensor
(Temperature & Humidity)
        -
        >
ESP32 Microcontroller
        -
        >
WiFi Network
        -
        >
Adafruit IO Cloud Platform
        -
        >
Dashboard & Serial Monitor


## Features
• Real-time temperature monitoring
• Real-time humidity monitoring
• Cloud data transmission via MQTT
• Wireless communication using ESP32
• Remote dashboard visualization
• Fully simulated IoT system


## Hardware Components
Component	Purpose
ESP32 DevKit V1	Main microcontroller
DHT22 Sensor	Temperature & humidity sensing
LED	        Output indicator
Resistor	Current limiting
Breadboard	Circuit assembly
Jumper wires	Electrical connections


## Software & Tools
Tool	        Purpose
Arduino IDE	Firmware development
Wokwi Simulator	ESP32 simulation
Adafruit IO	Cloud platform
GitHub	Version control


## Libraries used:

WiFi.h

AdafruitIO_WiFi.h

DHT.h


## How It Works

ESP32 connects to WiFi network

ESP32 connects to Adafruit IO cloud

DHT22 sensor measures environmental conditions

ESP32 publishes data every 5 seconds

Cloud dashboard updates in real time


## Example Output
Adafruit IO connected!
Temp: 36.7 C, Hum: 50.5 %
Temp OK, Hum OK


## Repository Structure
ENGR4321-ESP32-WiFi-Assignment
│
├── sketch.ino
├── README.md
└── images


## Engineering Skills Demonstrated

Embedded Systems
Internet of Things (IoT)
Wireless Communication
Cloud Integration
Sensor Integration
ESP32 Development


## Applications

Environmental monitoring
Smart home systems
Industrial monitoring
Remote sensing systems


## Author

Austin Davisson
Mechatronics Engineering Student
University of the Incarnate Word


