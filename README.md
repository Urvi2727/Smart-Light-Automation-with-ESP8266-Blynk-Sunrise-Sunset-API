# 🏠 Intelligent Home Light Automation using ESP8266, Blynk & Sunrise/Sunset API

An **IoT-based smart home lighting system** that automates lighting using an **ESP8266 (NodeMCU)**. The system combines **real-time sunrise/sunset scheduling**, **ambient light sensing**, and **remote mobile control** to provide an energy-efficient and adaptive lighting solution.

The project supports **dual automation modes**, allowing users to switch seamlessly between **API-based scheduling** and **LDR-based environmental sensing**, while also providing manual control through the **Blynk IoT platform**.

---

## ✨ Key Features

- 📱 Remote light control through the Blynk mobile application
- 🌅 Automatic scheduling using Sunrise/Sunset API based on geographical location
- 🌗 Ambient light detection using an LDR sensor
- 🔁 Dual automation modes with real-time switching
- 🎛️ Manual override available at any time
- 📡 Live monitoring through the Blynk dashboard
- ⚡ Energy-efficient operation by eliminating unnecessary lighting
- 🔧 Modular architecture that can be extended for additional smart home devices

---

# 🏗️ System Architecture

```
                 Light Sensor (LDR)
                        │
                        ▼
                ESP8266 (NodeMCU)
              ┌─────────┼──────────┐
              │         │          │
              ▼         ▼          ▼
         Blynk Cloud  Sunrise API  Relay Module
              │                     │
              └────────────┬────────┘
                           ▼
                     Home Lighting
```

---

## 🧰 Hardware Components

- ESP8266 NodeMCU
- LM393 + LDR Module
- Relay Module
- LED / AC Load
- Breadboard
- Jumper Wires
- USB Power Supply
- Wi-Fi Network

---

## 💻 Software & Technologies

- Arduino IDE
- ESP8266 Arduino Core
- Blynk IoT Platform
- REST API Integration
- C++
- Git & GitHub

---

# ⚙️ System Workflow

The controller continuously monitors the selected operating mode and performs lighting automation accordingly.

## 🌅 Mode 1 — Sunrise/Sunset Automation

- Retrieves sunrise and sunset timings using a REST API.
- Automatically turns lights ON after sunset.
- Automatically turns lights OFF after sunrise.
- Eliminates the need for fixed timers.

### Advantages

- Location-aware scheduling
- Automatically adapts to seasonal daylight changes
- No manual reconfiguration required

---

## 🌗 Mode 2 — Ambient Light Automation

- Continuously monitors surrounding light intensity using an LDR sensor.
- Turns lights ON when ambient light falls below the threshold.
- Turns lights OFF when sufficient natural light is available.

### Advantages

- Responds instantly to changing weather conditions
- More adaptive than time-based automation
- Conserves electrical energy

---

## 🎛️ Manual Control

The system also supports complete manual control through the Blynk application.

Users can:

- Turn lights ON/OFF remotely
- Switch between API and Sensor modes
- Monitor sensor values in real time

Manual commands always take priority over automation.

---

# 📱 Blynk Dashboard

The Blynk dashboard provides a centralized interface for monitoring and controlling the system.

## Widgets Used

| Widget | Virtual Pin | Function |
|---------|-------------|----------|
| Display | V1 | Displays LDR sensor readings |
| Switch | V2 | Manual Light Control |
| Switch | V3 | Toggle between API Mode and Sensor Mode |

---

# 🚀 Future Improvements

- MQTT-based communication
- Home Assistant integration
- Voice control using Google Assistant / Alexa
- Occupancy detection using PIR sensors
- Energy consumption analytics
- Weather-aware lighting automation
- AI-based predictive lighting schedules

---

# 🛠️ Getting Started

### Clone the Repository

```bash
git clone https://github.com/Urvi2727/Home-Light-Automation.git
cd Home-Light-Automation
```

### Install Dependencies

- Install ESP8266 Board Package
- Install the required Arduino libraries
- Create a Blynk Template
- Add your Auth Token
- Configure Wi-Fi credentials
- Upload the code to ESP8266

---

# 📈 Project Highlights

- Developed an IoT-based smart lighting automation system using ESP8266.
- Integrated REST APIs with embedded hardware for real-time scheduling.
- Implemented dual-mode automation combining environmental sensing and cloud-based scheduling.
- Enabled remote monitoring and control using the Blynk IoT platform.
- Designed a modular architecture that can be extended into a complete smart home ecosystem.

---

## 📄 License

This project is intended for educational and learning purposes.
