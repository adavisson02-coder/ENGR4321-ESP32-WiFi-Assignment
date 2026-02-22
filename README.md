# ESP32 WiFi Temperature and Humidity Monitoring using Adafruit IO
**Course:** ENGR 4321 – Microcontrollers and Embedded Systems  
**Student:** Austin Davisson  
**University:** University of the Incarnate Word  
**Assignment:** Simulation Assignment Report (SAR 3)

---

# Project Overview

This project demonstrates an Internet-connected embedded system using the ESP32 microcontroller. The system reads temperature and humidity data from a DHT22 sensor and sends the data to the Adafruit IO cloud platform using WiFi and MQTT communication.

The data is displayed in real-time on the Adafruit IO dashboard. This project demonstrates IoT concepts including wireless networking, cloud communication, and remote monitoring.

---

# System Block Diagram

DHT22 Sensor → ESP32 → WiFi → Adafruit IO Cloud Dashboard
|
LED (Cloud Controlled Output)


---

# Hardware Components

• ESP32 DevKit V1  
• DHT22 Temperature and Humidity Sensor  
• LED (GPIO 2)  
• Wokwi ESP32 Simulator  

---

# Software and Communication Description

## WiFi Connection

The ESP32 connects to the wireless network:

SSID: Wokwi-GUEST
Password: None


The WiFi connection allows the ESP32 to communicate with cloud services.

---

## Cloud Communication (API / MQTT)

The ESP32 communicates with Adafruit IO using the MQTT protocol.

Adafruit IO acts as the cloud server and stores the sensor data in feeds.

Feeds used:

temperature
humidity
led


The ESP32:

• Publishes temperature data to the temperature feed  
• Publishes humidity data to the humidity feed  
• Subscribes to the led feed to control the LED  

---

## Data Exchange

Sensor data is transmitted every 10 seconds.

Example:

Temperature: 24.00 C
Humidity: 40.00 %


The Adafruit IO dashboard updates in real time.

---

# Input and Output

## Input

DHT22 Sensor

Provides:

• Temperature
• Humidity

---

## Output

LED Indicator

Controlled remotely from Adafruit IO dashboard.

Serial Monitor

Displays system status and sensor readings.

Adafruit IO Dashboard

Displays live sensor data.

---

# Wokwi Simulation

Simulation Link:

(Paste your Wokwi share link here)

Example:

https://wokwi.com/projects/yourprojectlink

---

# Results

The system successfully:

• Connected to WiFi  
• Connected to Adafruit IO cloud  
• Read temperature and humidity data  
• Published data to cloud dashboard  
• Updated dashboard in real-time  
• Controlled LED from cloud  

---

# Screenshots

Insert screenshots in this section:

• Wokwi Circuit  
• Serial Monitor Output  
• Adafruit IO Dashboard  

---

# Conclusion

This project successfully demonstrated IoT cloud monitoring using the ESP32 microcontroller. The system was able to connect to WiFi, transmit sensor data to a cloud server, and display the information remotely.

This project demonstrates real-world embedded system and IoT communication principles.

---

# Repository Files

WeatherAdafruitIO.ino
diagram.json
README.md


---

# References

Adafruit IO Documentation  
https://io.adafruit.com/

SunFounder ESP32 Starter Kit Documentation  
https://docs.sunfounder.com/

Wokwi ESP32 Simulator  
https://wokwi.com/

---

# Author

Austin Davisson  
ENGR 4321  
University of the Incarnate Word
