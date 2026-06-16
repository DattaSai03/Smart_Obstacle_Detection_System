# Smart Obstacle Detection System for Visually Impaired Using Ultrasonic Sensors

An embedded systems project designed to assist visually impaired individuals by detecting nearby obstacles using ultrasonic sensors and providing real-time directional audio alerts through buzzers.

---

# 📌 Project Overview

The Smart Obstacle Detection System is developed using Arduino UNO, HC-SR04 Ultrasonic Sensors, and Directional Buzzers to help visually impaired individuals navigate safely.

The system continuously monitors obstacles in the:

- Left Direction
- Front Direction
- Right Direction

using three ultrasonic sensors.

The Arduino UNO processes all sensor readings using minimum-distance priority logic and activates the corresponding buzzer whenever an obstacle is detected within the predefined threshold distance of 300 cm.

This project demonstrates practical implementation of:

- Embedded Systems
- Sensor Interfacing
- Real-Time Processing
- Embedded C++ Programming
- Assistive Technology

---

# 🎯 Objectives

- Detect nearby obstacles in real time
- Identify the nearest obstacle
- Provide directional audio alerts
- Improve navigation safety for visually impaired individuals
- Implement minimum-distance priority logic
- Demonstrate embedded systems concepts practically

---

# ✨ Features

- Real-time obstacle detection
- Direction-based buzzer indication
- Priority-based obstacle identification
- Threshold-based detection (300 cm)
- Continuous monitoring system
- Fast response and stable operation
- Virtual implementation using simulation software
- Simple and cost-effective design

---

# 🛠️ Components Used

| Component | Quantity |
|---|---|
| Arduino UNO R3 | 1 |
| HC-SR04 Ultrasonic Sensor | 3 |
| Buzzers | 3 |
| Breadboard | 1 |
| Jumper Wires | Multiple |

---

# 🔌 Pin Connections

| Component | Arduino Pin |
|---|---|
| Left Sensor TRIG | D2 |
| Left Sensor ECHO | D3 |
| Front Sensor TRIG | D4 |
| Front Sensor ECHO | D5 |
| Right Sensor TRIG | D6 |
| Right Sensor ECHO | D7 |
| Left Buzzer | D8 |
| Front Buzzer | D9 |
| Right Buzzer | D10 |

---

# ⚙️ Working Principle

1. Ultrasonic sensors continuously detect nearby obstacles.
2. Arduino UNO reads all sensor distances.
3. The minimum distance is identified.
4. The threshold condition (300 cm) is checked.
5. The corresponding buzzer is activated.
6. The process continuously repeats in real time.

---

# 🧠 Core Logic Used

The system compares:

- Left Distance
- Front Distance
- Right Distance

and identifies the nearest obstacle using:

```cpp
min(frontDist, min(leftDist, rightDist));
```

## Priority Logic

```text
Front > Left > Right
```

If multiple distances are equal:
- Front gets highest priority
- Then Left
- Then Right

This improves navigation safety because front obstacles are more critical during walking.

---

# 💻 Software Used

- Arduino IDE
- Wokwi Simulator
- Embedded C++

---

# 📊 System Flow

```text
Start
   ↓
Read Sensor Distances
   ↓
Compare All Distances
   ↓
Find Minimum Distance
   ↓
Check Threshold (≤ 300 cm)
   ↓
Activate Corresponding Buzzer
   ↓
Repeat Continuously
```

---

# 📷 Project Diagrams

The project includes:

- Flow Chart

  <img width="1024" height="1536" alt="ChatGPT Image Jun 11, 2026, 10_21_32 AM" src="https://github.com/user-attachments/assets/75d8c353-8c20-4358-ac51-94d1a3bbe75c" />

- Block Diagram

  <img width="1536" height="1024" alt="ChatGPT Image Jun 11, 2026, 10_23_51 AM" src="https://github.com/user-attachments/assets/ba26301d-7f54-49ec-a197-71f731a0d5aa" />

- Schematic Diagram

<img width="1536" height="1024" alt="ChatGPT Image Jun 16, 2026, 10_56_29 AM" src="https://github.com/user-attachments/assets/ebb0fe74-5781-4e18-beee-790fc821f0fa" />

---

# 🚀 Future Scope

- Add vibration motor alerts
- Add voice guidance system
- Add GPS tracking
- Add AI-based obstacle recognition
- Develop wearable implementation
- Integrate IoT monitoring features

---

# 📈 Results

The system successfully detected nearby obstacles in real time and activated the appropriate directional buzzer based on minimum-distance priority logic. The simulation demonstrated stable performance, fast response time, and reliable obstacle detection within the predefined threshold distance.

---

# 🧩 Skills Used

- Embedded Systems
- Arduino Programming
- Embedded C++
- Ultrasonic Sensor Interfacing
- Real-Time Systems
- Sensor Integration
- Hardware Interfacing
- Circuit Design

---

# 👨‍💻 Author

## Devulapalli Datta Sai Srinivas

B.Tech – Electronics and Communication Engineering  
Vellore Institute of Technology – Andhra Pradesh

---

# 🏢 Internship

Submitted To:

## Maven Silicon  
VLSI & Embedded Systems Training Institute

---
