ENGR4321 – ESP32 WiFi Assignment

Simulation Assignment 3: ESP32 WiFi, APIs, and Cloud Data
Student: Austin Davisson
Course: ENGR 4321 Microcontrollers and Embedded Systems
Date: February 23, 2026

Project Overview

This project demonstrates an Internet of Things (IoT) embedded system using the ESP32 microcontroller in the Wokwi simulator. The ESP32 connects to a WiFi network and communicates with the Adafruit IO cloud platform to transmit environmental sensor data.

A DHT22 temperature and humidity sensor is used as the input device. The ESP32 reads the sensor values and publishes the data to the Adafruit IO cloud dashboard every five seconds. This allows real-time remote monitoring of environmental conditions.

This project demonstrates key IoT concepts including WiFi networking, cloud communication, and sensor integration.

System Block Diagram
DHT22 Sensor
(Temperature and Humidity)
        │
        │ GPIO 13
        ▼
ESP32 Microcontroller
(WiFi Enabled Device)
        │
        │ WiFi Connection
        ▼
Adafruit IO Cloud Platform
(MQTT / JSON Data Transfer)
        │
        ▼
Cloud Dashboard and Serial Monitor

WiFi and API Interaction Description

The ESP32 connects to the internet using the built-in WiFi module and the WiFi.h library. In the Wokwi simulation environment, the ESP32 connects to the network named:

Wokwi-GUEST


After establishing a WiFi connection, the ESP32 communicates with the Adafruit IO cloud platform using the AdafruitIO_WiFi library.

Adafruit IO acts as a cloud API service that allows devices to send and receive data. The ESP32 sends temperature and humidity data to Adafruit IO feeds named:

temperature

humidity

The data is transmitted using the MQTT protocol, which internally uses JSON-formatted messages to exchange information between the ESP32 and the cloud server.

This allows the sensor data to be viewed remotely in real time on the Adafruit IO dashboard.

The Serial Monitor also displays confirmation messages showing successful data transmission.

Example output:

Adafruit IO connected!
Temp: 36.7 C, Hum: 50.5 %
Temp OK, Hum OK

Input and Output

Input Device:

DHT22 Temperature and Humidity Sensor

Output Devices:

Serial Monitor
Adafruit IO Cloud Dashboard
LED indicator

Wokwi Simulation Link

[https://wokwi.com/projects/YOUR-PROJECT-LINK](https://wokwi.com/projects/456615498165739521)

<img width="551" height="608" alt="Screenshot 2026-02-21 at 7 26 16 PM" src="https://github.com/user-attachments/assets/15a754ed-2318-49bf-b42f-78bdc07e103c" />


Summary

This project successfully demonstrated WiFi communication between an ESP32 and a cloud platform. The ESP32 collected sensor data and transmitted it to Adafruit IO, allowing real-time remote monitoring. This confirms proper operation of an IoT embedded system using cloud communication.
