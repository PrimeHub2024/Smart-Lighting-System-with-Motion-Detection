# 💡 Smart Lighting System with Motion Detection (SLSMD)

An intelligent and energy-efficient lighting system built using the **STM32 Nucleo** development board. The system automatically controls lighting based on **motion detection** and **ambient light intensity**, helping reduce unnecessary power consumption while improving user convenience.

---

## 📌 Project Overview

The **Smart Lighting System with Motion Detection (SLSMD)** is an embedded systems project that combines a **Passive Infrared (PIR) Sensor**, **Light Dependent Resistor (LDR)**, and **STM32 Nucleo** microcontroller to automate lighting.

The system continuously monitors:

- Human motion using a PIR sensor
- Ambient light intensity using an LDR

The LEDs are turned ON when:

- Motion is detected, or
- The surrounding environment is dark.

Otherwise, the LEDs remain OFF, ensuring efficient energy utilization.

---

## ✨ Features

- Motion-based automatic lighting
- Ambient light detection using LDR
- Energy-efficient operation
- Automatic LED control
- Real-time monitoring through Serial Monitor
- Simple and modular embedded system design

---

## 🛠 Hardware Components

- STM32 Nucleo Board
- PIR Motion Sensor
- LDR (Light Dependent Resistor)
- LEDs (3)
- Current Limiting Resistors
- Breadboard
- Jumper Wires
- USB Cable

---

## 💻 Software Used

- STM32 Arduino Core
- Arduino IDE
- Serial Monitor

---

## ⚙ Working Principle

1. The STM32 continuously reads the LDR analog value.
2. The PIR sensor monitors human movement.
3. If motion is detected:
   - All LEDs immediately turn ON.
4. If no motion is detected:
   - The LDR value is checked.
   - If the environment is dark, LEDs remain ON.
   - Otherwise, LEDs are turned OFF.
5. The process repeats continuously.

---

## 🔄 System Flow

```text
Start
   │
   ▼
Initialize STM32
   │
   ▼
Read PIR Sensor
   │
   ├── Motion Detected?
   │       │
   │      Yes
   │       │
   │       ▼
   │   Turn ON LEDs
   │       │
   │       ▼
   │    Repeat
   │
   ▼
Read LDR Value
   │
   ├── Low Light?
   │       │
   │      Yes
   │       │
   │       ▼
   │   Turn ON LEDs
   │
   └── No
           │
           ▼
      Turn OFF LEDs
           │
           ▼
         Repeat
```

---

## 📂 Project Structure

```text
Smart-Lighting-System-with-Motion-Detection
│
├── README.md
│
└── SLSMD
    ├── Final Circuit.PNG
    ├── Final Code.txt
    ├── Final Simulation.mp4
    │
    ├── Motion Detection using STM32 Nucleo
    │   ├── Screenshot of Output.jpeg
    │   ├── Simulation Video.mp4
    │   └── The Codee.txt
    │
    └── Lighting System using STM32 Nucleo
        ├── Screenshot of Output.PNG
        ├── Simulation Video.mp4
        └── The Code.txt
```

---

## 🧠 Program Logic

The system prioritizes **motion detection**.

- If motion is detected:
  - All LEDs are switched ON.
- Otherwise:
  - The LDR value is evaluated.
  - Low light → LEDs ON
  - Bright light → LEDs OFF

This approach ensures that lighting is only active when required, reducing unnecessary power consumption.

---

## 🚀 Applications

- Smart Homes
- Office Automation
- Corridors
- Staircases
- Parking Areas
- Smart Buildings
- Energy Saving Systems

---

## 🔮 Future Improvements

- IoT-based remote monitoring
- Mobile application integration
- Adjustable brightness using PWM
- Occupancy analytics
- Voice assistant integration
- Cloud data logging

---

## 📸 Project Demonstration

The repository includes:

- Circuit diagram
- Source code
- Simulation videos
- Output screenshots

---

## 👨‍💻 Author

**Aadesh Anil Labde**

Electronics & Telecommunication Engineering

Interested in:

- Embedded Systems
- IoT
- PCB Design
- Robotics
- Automation
- Hardware Design

---

## 📄 License

This project is intended for educational and academic purposes.
