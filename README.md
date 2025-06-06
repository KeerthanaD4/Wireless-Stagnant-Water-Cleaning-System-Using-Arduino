# 🌊 Wireless Stagnant Water Cleaning System Using Arduino

A Bluetooth-controlled, sensor-integrated robotic solution to monitor and clean stagnant water bodies like ponds and lakes. This project leverages Arduino, IoT sensors, and wireless communication to collect floating garbage and assess water quality in real-time.

## 🚀 Project Overview

Water pollution, especially in stagnant water bodies, poses a significant threat to ecosystems and public health. This system addresses the issue using an Arduino-powered floating bot equipped with:
- Garbage collection roller (PVC + conveyor mechanism)
- TDS and Turbidity sensors for real-time water quality monitoring
- Bluetooth control via mobile application (Serial Bluetooth Terminal)

## 🧠 Features

- 🛥️ Wireless Bluetooth control for forward/backward/left/right/stop/start movements
- 🧹 Automated garbage collection using a PVC roller mechanism
- 📊 Real-time monitoring of:
  - **Turbidity** (suspended particles)
  - **TDS (Total Dissolved Solids)**
- ⚙️ Arduino-based, low-cost, scalable and eco-friendly solution

## 🛠️ Components Used
### Hardware
- Arduino UNO
- Bluetooth Module (HC-06)
- Motor Driver (L298N)
- BO Motors (300 RPM x4)
- PVC pipe-based float structure
- TDS Sensor (V1.0)
- Turbidity Sensor
- 12V Solar Panel (optional)
- 3.7V, 2600mAh Battery
- LM2596 Buck Converter
- Jumper wires, Net, and Skimmer

### Software
- Arduino IDE (C Programming)
- Serial Bluetooth Terminal
- Android mobile with Bluetooth support

## 🧩 System Architecture
- **Input**: User sends commands (`M1`–`M6`) via mobile app
- **Control**: Arduino controls motor directions using L298N
- **Sensors**: TDS (Analog), Turbidity (Analog)
- **Output**: Sensor values are printed via Bluetooth terminal

## 🔧 Commands Used
| Command | Action             |
|---------|--------------------|
| M1      | Start device        |
| M2      | Move Forward        |
| M3      | Move Backward       |
| M4      | Turn Right          |
| M5      | Turn Left           |
| M6      | Stop device         |

## 🔄 System Workflow
1. User pairs mobile with HC-06 module via Bluetooth
2. Sends control commands using the app
3. Boat navigates and collects garbage
4. Sensors read real-time data
5. Data is displayed on the app

## 📷 Images
![image](https://github.com/user-attachments/assets/3d0f7a88-4b2f-42ff-97d7-7b95c08180ea)
![image](https://github.com/user-attachments/assets/65c46d08-33cb-4585-8b0d-50fa6fdadced)

## 🧪 Testing
| Test Case ID | Description                              | Status |
|--------------|------------------------------------------|--------|
| TC-01        | Arduino boot and Bluetooth connection     | ✅ Pass |
| TC-02        | Forward and directional control           | ✅ Pass |
| TC-03        | Garbage collection mechanism              | ✅ Pass |
| TC-04        | TDS sensor reading                        | ✅ Pass |
| TC-05        | Turbidity sensor reading                  | ✅ Pass |
| TC-06        | Operation in high weed density            | ❌ Fail |

## 📌 Future Enhancements
- Integrate solar charging and GPS navigation
- Add AI-based obstacle avoidance
- Use Wi-Fi or LoRa for long-range monitoring
- Enable automatic alerts via mobile or SMS

## 📄 License
This project is licensed under the [MIT License](LICENSE).
