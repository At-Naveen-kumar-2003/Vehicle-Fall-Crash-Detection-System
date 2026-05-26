# 🚗 Vehicle Fall & Crash Detection System

A real-time IoT-based Vehicle Fall & Crash Detection and V2V Alert System developed using ESP32, Raspberry Pi, LoRa, and Flask for intelligent vehicle safety monitoring and emergency alert generation.

---

## 📌 Project Overview

This project detects vehicle crashes, falls, gas leaks, and abnormal driving conditions in real time using multiple sensors and edge computing techniques. The system uses LoRa communication for long-range wireless data transmission and Raspberry Pi for local processing, monitoring, and alert generation.

The system also supports Vehicle-to-Vehicle (V2V) alert communication to notify nearby vehicles during emergency situations.

---

## ✨ Features

- 🚨 Real-time Crash & Fall Detection
- 📡 Long-Range LoRa Communication
- 🌍 GPS Location Tracking
- ⚡ Edge Computing using Raspberry Pi
- 📊 Live Flask Dashboard Monitoring
- 📧 Automatic Email Alert System
- 🔒 XOR Encryption & CRC Validation
- 🚗 Vehicle-to-Vehicle (V2V) Alerts
- 🗄️ SQLite Database Logging
- ☁️ Remote Dashboard Access using ZeroTier

---


## 🛠️ Hardware Components

- ESP32 Development Board
- Raspberry Pi 5
- SX1278 LoRa Module
- MPU6050 Accelerometer & Gyroscope
- MQ-135 Gas Sensor
- BME280 Environmental Sensor
- NEO-6M GPS Module
- OLED Display

---

## 💻 Software & Technologies

- Embedded C
- Python
- Flask
- SQLite
- LoRa Communication
- ESP32 Firmware
- Raspberry Pi
- HTML/CSS
- ZeroTier VPN

---

## ⚙️ System Workflow

1. ESP32 collects sensor and GPS data.
2. Data is encrypted and transmitted using LoRa.
3. Raspberry Pi receives and processes the data.
4. Fault detection algorithms identify crash/fall events.
5. Alerts are displayed on the Flask dashboard.
6. Email notifications are sent during emergencies.
7. Alert status is forwarded to nearby vehicles.

---

---

# 📂 Project File Description

## 1️⃣ Sender Node (`sender_node.ino`)

The Sender Node is developed using ESP32 and multiple sensors to collect real-time vehicle data such as acceleration, gas concentration, environmental conditions, and GPS location. The ESP32 processes the sensor values, detects abnormal conditions like crash or fall events, and transmits the encrypted data using LoRa communication.

### Main Functions
- Sensor data acquisition
- Crash & fall detection
- GPS tracking
- Gas leak monitoring
- LoRa data transmission
- Real-time event generation

---

## 2️⃣ Edge Receiver Node (`edge_receiver.py`)

The Edge Receiver Node runs on Raspberry Pi and acts as the central processing unit of the system. It receives LoRa packets from the ESP32 sender node, processes the data, stores it in the SQLite database, performs fault analysis, and triggers emergency alerts when abnormal events are detected.

### Main Functions
- LoRa packet reception
- Edge computing & fault analysis
- Database storage
- Email alert generation
- Data processing & monitoring
- Flask dashboard integration

---

## 3️⃣ Receiver Display Node (`receiver_display.ino`)

The Receiver Display Node receives processed alert messages from the Edge Node through LoRa communication and displays vehicle status information on an OLED display. This node enables Vehicle-to-Vehicle (V2V) communication for nearby vehicle alert notification.

### Main Functions
- Receive V2V alert messages
- Display crash/fall alerts
- Show real-time vehicle status
- OLED display visualization
- Nearby vehicle warning system

---

## 4️⃣ Flask Dashboard (`app.py`)

The Flask Dashboard provides a web-based monitoring interface for visualizing live vehicle data, alerts, GPS information, and stored records from the SQLite database.

### Main Functions
- Live dashboard visualization
- Real-time sensor monitoring
- Alert display system
- Database record visualization
- Vehicle status monitoring

---

## 5️⃣ Database Module (`database.py`)

The Database Module stores all received vehicle sensor data and event information using SQLite for future analysis and monitoring.

### Main Functions
- Store sensor data
- Save alert history
- Maintain vehicle records
- Support dashboard visualization
- Local data logging

---

## 📈 Results

- Real-time accident detection achieved
- Low latency communication
- Reliable long-range LoRa transmission
- Successful dashboard visualization
- Real-time GPS tracking and alert generation

---

## 🎯 Applications

- Smart Vehicle Safety Systems
- Fleet Monitoring
- Emergency Alert Systems
- V2V Communication
- IoT-Based Automotive Solutions

---

## 📚 Skills Practiced

- Embedded Systems Development
- ESP32 Programming
- Sensor Interfacing
- LoRa Communication
- Edge Computing
- Flask Dashboard Development
- Real-Time Monitoring
- Embedded Firmware Development

---

## 👨‍💻 Author

Naveen Kumar S  
M.Tech Embedded Systems Engineering  
Amrita Vishwa Vidyapeetham
