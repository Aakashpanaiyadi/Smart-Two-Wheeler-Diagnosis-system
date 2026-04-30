# Smart-Two-Wheeler-Diagnosis-system


 Smart Two-Wheeler EV Diagnosis System (IoT Based)
 Project Overview

This project is an IoT-based smart diagnosis system for a two-wheeler electric vehicle (EV).
It continuously monitors key EV parameters such as motor current, motor voltage, motor temperature, battery current, battery voltage, and battery temperature, and displays the live data on a web dashboard using Firebase Realtime Database.

The system also provides predefined troubleshooting guidance for common EV faults such as battery not charging, motor not working and overheating ,helping users and technicians identify issues quickly.

System Architecture

Arduino Uno acts as the data acquisition unit.

ESP8266 (NodeMCU) acts as the IoT gateway.

Firebase Realtime Database is used for cloud data storage.

HTML Web Dashboard displays live readings and troubleshooting steps.

Hardware Description
Arduino Side

Potentiometers are used to simulate real EV sensors:

Motor Current

Motor Voltage

Motor Temperature

Battery Current

Battery Voltage

Battery Temperature

Analog sensor values are mapped to realistic EV operating ranges.

Sensor data is formatted as a comma-separated string with start < and end > markers.

Data is transmitted to ESP8266 via UART (Serial Communication).

ESP8266 Side

Receives sensor data from Arduino via UART.

Parses and validates incoming data.

Uploads structured data to Firebase Realtime Database using JSON format.

Maintains Wi-Fi reconnection and reliable cloud communication.

Cloud & Web Interface

Firebase Realtime Database stores live EV sensor data.

A custom HTML web page fetches and displays real-time values.

Live parameters update automatically without page refresh.

Troubleshooting section provides predefined fault-handling steps for:

Battery not charging

Motor not running

Battery overheating 






HARDWARE 




<img width="641" height="852" alt="image" src="https://github.com/user-attachments/assets/ed438ee7-bdfa-4c82-94e3-9802c8bcd930" />



HTML WEB PAGE



<img width="1875" height="915" alt="image" src="https://github.com/user-attachments/assets/ee61258c-d0d9-494f-8dfd-5ac3a76d194c" />


