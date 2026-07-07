# Telematics System with Accident Detection
**Usage-Based Vehicle Insurance (UBI)**  
**Harare Institute of Technology | BT (Hons) Electronic Engineering Capstone | May 2020**

## Overview
Designed and implemented a full-stack telematics system for usage-based motor 
insurance with real-time accident detection. The system collects driving behavior 
data (GPS location, speed, G-force, acceleration) via hardware sensors on a 
Raspberry Pi and transmits to a cloud database via MQTT, displaying results on 
an insurance web dashboard.

## System Architecture
## Hardware Components
- **Controller:** Raspberry Pi 4 Model B
- **GPS:** Neo-6MV (UART serial communication)
- **IMU:** MPU6050 GY-512 — 6-axis (3-axis gyroscope + 3-axis accelerometer, I2C)
- **Speed sensor:** LM393 (digital input)
- **Motor driver:** L298N Dual H-Bridge
- **Platform:** RC car with remote control (FS-iA6 receiver)

## Software Stack
- **Embedded:** Python (sensor interfacing, MQTT publishing, accident detection logic)
- **Backend:** Node.js + Express (REST API, MongoDB aggregation pipelines)
- **Database:** MongoDB Atlas on AWS
- **Frontend:** JavaScript web dashboard (gyroscope charts, GPS tracker, driving meters)
- **Notifications:** Nodemailer (email alerts) + Web Push API (browser notifications)
- **Simulation:** Proteus (circuit design and simulation)

## Key Features
- Real-time GPS vehicle tracking dashboard
- Accelerometer and gyroscope data visualization
- Automated accident detection via G-force threshold monitoring
- Good/Bad driving score calculation using MongoDB aggregation pipelines
- Automated email and push notification alerts on accident detection
- 99.9% server uptime on AWS deployment

## Results
| Action | Output |
|--------|--------|
| Engine ON | Telematics device boots, connects to cloud |
| GPS active | Coordinates streamed to MongoDB |
| Normal driving | Driver behavior score calculated |
| Accident detected | Email + push alert sent to insurer dashboard |

## Stack
`Python` `Raspberry Pi` `MQTT` `MongoDB` `Node.js` `AWS` `JavaScript` 
`GPS (Neo-6MV)` `MPU6050` `I2C` `UART` `REST API`
