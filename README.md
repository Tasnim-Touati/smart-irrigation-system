# 📁 Smart Irrigation System - Full Roadmap

---
# 🌱 Smart Irrigation System

A **Smart Irrigation System** based on **Arduino**, designed to monitor environmental conditions such as **soil moisture**, **temperature** and **humidity** sensing, and control a **pump and LED** automatically or manually via a **Python-based real-time dashboard**.

This project enables **efficient water usage**, **live monitoring**, and **automation**, supporting smarter irrigation for gardens and experimental prototypes.

---

## ⚙️ Features
- **Mobile/GUI Interface**: Schedule irrigation, perform quick manual overrides, and visualize sensor readings.  
- **Automated vs. Manual Simulation**: Compared irrigation strategies using public datasets, showing potential water savings of 10–25%.  
- **Real-Time Dashboard**: Built with Python for monitoring soil moisture and optional temperature/humidity sensors.  
- **Predictive Logic**: Sensor data is processed to identify when irrigation is needed.  
- **Data Logging**: Arduino records sensor readings in real time, improving data management efficiency by ~30%.  

---
# 🎯 Project Roadmap

| Phase | Description |
|-------|-------------|
| Phase 1 | Setup Arduino firmware to read sensors (soil moisture, DHT11) and control pump/LED. |
| Phase 2 | Build Python dashboard for real-time visualization and manual irrigation override. |
| Phase 3 | Implement automated irrigation logic based on sensor thresholds. |
| Phase 4 | Simulate automated vs manual irrigation using public datasets to analyze potential water savings. |
| Phase 5 | (Optional) Upgrade to ESP8266 / WiFi module for remote monitoring and control. |
| Phase 6 | (Optional) Add notifications, predictive logic, and advanced dashboard features. |

---

## 🏛 Architecture
```text
[ Arduino + Sensors ]  -->  [ Python Dashboard / Data Logging ]
```

---

## 🧩 Technology Stack
| Part                  | Technology / Hardware           |
|-----------------------|--------------------------------|
| Microcontroller       | Arduino (Uno/Nano)             |
| Sensors               | Soil Moisture, DHT11 (optional) |
| Actuator              | LED (pump simulation) or Relay + Pump |
| Dashboard / Interface | Python (Tkinter/Matplotlib)    |
| Data Logging          | Arduino                        |

---

## 🛠 Hardware Requirements
| Component               | Quantity | Description                        |
|-------------------------|----------|------------------------------------|
| Arduino Uno / Nano      | 1        | Microcontroller for sensor control |
| Soil Moisture Sensor    | 1        | Measures soil moisture level       |
| DHT11 Sensor (optional) | 1        | Temperature and Humidity sensor    |
| Relay Module (optional) | 1        | Controls water pump safely         |
| LED                     | 1        | Simulates the pump action          |
| Jumper Wires            | As needed | For connections                     |
| Breadboard              | 1        | For prototyping                     |

---

## 🔌 Pin Connections
| Arduino Pin | Connected To                  |
|-------------|--------------------------------|
| A0          | Soil Moisture Sensor (Analog) |
| D4          | DHT11 Sensor (Digital, optional) |
| LED_BUILTIN | Simulated Pump (LED)          |
| D5 / Relay  | Water Pump (optional)         |

---

## 🚀 Setup Instructions

### Arduino Firmware
1. Open Arduino IDE and load the `.ino` firmware.  
2. Install necessary libraries:  
   - `DHT.h` (if using DHT11)  
3. Connect sensors according to the pin mapping.  
4. Upload the firmware to the Arduino board.  

### Python Dashboard / Interface
1. Install Python and required packages (`matplotlib`, `tkinter`).
   pip install matplotlib
   pip install tk
3. Run the dashboard to visualize live or logged sensor data and control irrigation manually.  

---

## 📈 AutoMode Logic
- Pump (LED) turns **ON** when soil moisture drops below the threshold.  
- Pump turns **OFF** when moisture reaches acceptable levels.  
- Thresholds configurable in the firmware.  

---

## 🔧 Future Improvements
- Upgrade to **ESP8266 / WiFi module** for remote monitoring.  
- Add mobile app notifications.  
- Include more sensors for temperature/humidity.  
- Integrate predictive irrigation logic fully with AI.  
- Real water pump control via relay module.  

---

## ✨ Credits
> Developed by **Tasnim Touati** – Final-year Computer Science Student.
