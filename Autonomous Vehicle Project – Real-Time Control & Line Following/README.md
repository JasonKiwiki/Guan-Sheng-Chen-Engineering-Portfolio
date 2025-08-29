# Autonomous Vehicle Project – Real-Time Control & Line Following

## Overview
This project (Sessions I–IV of the Applied Electrical & Electronic Engineering construction labs) involved designing and building a four-wheel autonomous robotic vehicle with **Arduino-based control, HMI (Human–Machine Interface), real-time motion sensing, wireless communication, and multi-sensor line following**.  

The work spanned from basic motor drivers to advanced PID control with optical sensors, integrating both **hardware circuit design** and **firmware development**.

---

## Features
- **Session 1–2:**  
  - Implemented H-bridge motor driver for bidirectional control.  
  - Designed real-time system operation (RT sinewave generator).  
  - Built HMI with LCD, encoder, buzzer, and buttons for vehicle status monitoring.  
  - Established serial communication between dual Arduino microcontrollers.  

- **Session 3–4:**  
  - Integrated **MPU-6050 accelerometer & gyroscope** for motion sensing.  
  - Developed **wireless communication** using nRF24L01 (RF) and HC-06 (Bluetooth), enabling remote control via joystick or smartphone.  
  - Constructed a **logic gate interface board** with 74-series ICs.  
  - Implemented **line following** using TCRT5000 optical sensors (Bang-bang control).  
  - Advanced to **PID-controlled line following** with SF-8CHIDTS 8-channel module, achieving smooth trajectory tracking.  
  - Designed HMI for **real-time PID parameter tuning** and LCD status display.  

---

## Technical Stack
- **Hardware:** Arduino Nano, MPU-6050 IMU, nRF24L01, HC-06 Bluetooth, TCRT5000, SF-8CHIDTS, LCD1602, H-bridge motor driver.  
- **Software:** Arduino IDE (C/C++), PWM control, serial communication protocols (UART, I2C, SPI).  
- **Control Methods:** Bang-bang control, PID tuning, real-time system operation.  

---

## Results
- Successfully built and tested a 4-wheel vehicle platform with:  
  - >200 Hz real-time control loop frequency.  
  - Stable wireless communication for remote operation.  
  - Smooth PID-based line following with multi-sensor fusion.  
- Demonstrated robust integration of **control theory, digital logic, and embedded programming**.  
- Provided a foundation for advanced autonomous vehicle design.  

---

## Related Area
Arduino Firmware Development • PID Control • Real-Time Control • Wireless Communication • Motion Sensing • Sensor Integration • Digital Logic Design • Robotics System Control  

---
📌 *Note: Reports and circuit diagrams are included in `/reports/` for reference. This repository is for portfolio demonstration; full source code available upon request.*
