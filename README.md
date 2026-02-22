ESP32 WiFi Temperature and Humidity Monitoring System

Course: ENGR 4321 Microcontrollers & Embedded Systems
Student: Austin Davisson
Date: February 2026

Project Overview

This project demonstrates an Internet-connected environmental monitoring system using an ESP32 DevKit V1 and a DHT22 temperature and humidity sensor. The ESP32 connects to a WiFi network and transmits sensor data to the Adafruit IO cloud platform. The system allows real-time monitoring of environmental conditions through a cloud dashboard and the Serial Monitor.

Hardware Components (Simulated)

ESP32 DevKit V1

DHT22 Temperature and Humidity Sensor

LED

Resistor

Breadboard

Jumper Wires

Simulation Link

[https://wokwi.com/projects/456615498165739521](https://wokwi.com/projects/456615498165739521)
<img width="486" height="537" alt="Screenshot 2026-02-21 at 7 37 25 PM" src="https://github.com/user-attachments/assets/84d717b6-bc0e-45e2-bbf4-c03fe06dfdfc" />


How It Works

The ESP32 connects to the Wokwi-GUEST WiFi network using its built-in wireless module. Once connected, it establishes communication with the Adafruit IO cloud service using the MQTT protocol.

The DHT22 sensor continuously measures temperature and humidity. The ESP32 reads these values every five seconds and publishes the data to Adafruit IO feeds named:

temperature

humidity

The cloud dashboard displays the data in real time, allowing remote monitoring.

The Serial Monitor also confirms successful data transmission and displays the sensor readings.

Example Serial Output
Adafruit IO connected!
Temp: 36.7 C, Hum: 50.5 %
Temp OK, Hum OK

System Block Diagram
DHT22 Sensor
(Temperature / Humidity)
        │
        ▼
ESP32 Microcontroller
(WiFi Connection)
        │
        ▼
Adafruit IO Cloud
        │
        ▼
Dashboard / Serial Monitor

Repository Contents

sketch.ino – ESP32 source code

README.md – Project documentation

Summary

This project successfully demonstrated WiFi communication between an ESP32 and a cloud platform. Sensor data was collected and transmitted to Adafruit IO, confirming proper operation of an Internet-connected embedded system.
