# MediLoRa
This repository contains the firmware and Node-RED configuration for a Smart Health Monitoring System that utilizes LoRa-Dino modules for long-range, internet-independent communication between a patient-side transmitter and a nursing station receiver.

**Project Overview**
The system continuously monitors vital health parameters and transmits data wirelessly using LoRa-Dino. The receiver processes this data, triggers emergency alerts if abnormal readings are detected, and displays real-time values on a Node-RED dashboard for medical staff.

**Features**
✅ Wireless health monitoring system using LoRa-Dino
✅ Sensors for ECG, GSR, and DS18B20 (temperature)
✅ Emergency alerts via buzzer and LED
✅ Real-time monitoring with Node-RED
✅ Data transmission without internet dependency

**Files in This Repository**
**_1. lora_sender.ino_**
Code for the LoRa-Dino transmitter (patient-worn device)
Reads sensor data and transmits it via LoRa
**_2. lora_receiver.ino_**
Code for the LoRa-Dino receiver (nursing station)
Receives sensor data and triggers alerts when necessary
**_3. flows.json_**
Node-RED flow file for real-time data visualization and monitoring
Displays temperature, GSR, and ECG values
Integrates with MQTT for data processing
