# 🔐💡🌧️ Arduino-Based Integrated Smart Home System

### Team Members:
- Shefali Bishnoi (2301CS87)
- Juhi Sahni (2301CS88)
- Saniya Prakash (2301CS49)
- Manvitha Reddy (2301CS29)

---

## 🏠 Project Overview

This project integrates three key smart home modules into a single Arduino-based automation system:

1. 🔒 **Home Security & Fire Detection System**
2. 🌧️ **Rainwater Harvesting System**
3. 💡 **Motion-Activated Smart Lighting**

All systems operate concurrently and share hardware resources efficiently, while being monitored via serial communication.

---

## 🎯 Motivation

- ✅ Promote **resource efficiency** by combining multiple home systems on one microcontroller.
- ✅ Ensure **safety and security** through real-time intrusion and fire detection.
- ✅ Encourage **sustainability** via rainwater harvesting.
- ✅ Achieve **energy conservation** using motion-based smart lighting.

---

## 🚀 Key Features & Innovations

- 🔁 **Non-blocking operation** — All systems run in parallel without delay() functions.
- 🔒 **Access code authentication** — Only authorized users can unlock the door.
- 🔥 **Fire emergency handling** — Auto-unlocks door and sounds buzzer if fire is detected.
- 🌧️ **Adaptive rainwater control** — Automatically opens/closes water valve based on rain intensity and tank level.
- 💡 **Motion-triggered lighting** — Lights switch on when movement is detected; turn off after inactivity.
- ⚙️ **Debounced sensor readings** — Prevents false positives from noisy sensor data.
- 🧠 **Graceful servo control** — Smooth transitions extend servo motor life and offer visual feedback.

---

## 🔌 Hardware Components

| Component                 | Quantity |
|---------------------------|----------|
| Arduino UNO               | 1        |
| Ultrasonic Sensors        | 2        |
| IR Sensor                 | 1        |
| Flame Sensor              | 1        |
| Servo Motors              | 2        |
| Red, Green, Blue LEDs     | 3        |
| Piezo Buzzer              | 1        |
| Rain Sensor (Analog)      | 1        |
| Water Level Sensor        | 1        |
| Breadboard + Jumpers      | 1 set    |
| NTC Thermistor            | 1        |

---

## 🧩 System Architecture

### 🔐 Security & Fire Detection
- Detects motion using IR and Ultrasonic sensors.
- Password-verified door unlocking.
- Monitors fire via flame sensor + NTC thermistor.
- Triggers buzzer and unlocks doors in emergencies.

### 🌧️ Rainwater Harvesting
- Monitors rainfall and tank levels.
- Controls water valve using servo.
- Prevents overflow and saves rainwater.

### 💡 Smart Lighting System
- Detects presence using ultrasonic sensor.
- Activates light only when motion is detected.
- Auto shut-off after inactivity to save energy.

---

## 🛠️ Code Structure

Each subsystem includes:
- `initialize*()` – Pin setup and component initialization.
- `update*()` – Logic loop for sensor handling and control.
- Custom utility functions for:
  - Servo transitions
  - Debouncing
  - Fire detection logic
  - Access code validation

---

## 📈 Project Outcome

- ✅ Successfully combined security, fire detection, lighting, and water management in one system.
- ✅ Maintained real-time performance with non-blocking architecture.
- ✅ Improved environmental sustainability and energy efficiency.

---

## 👩‍💻 Individual Contributions

| Team Member       | Contribution                                                                 |
|-------------------|------------------------------------------------------------------------------|
| **Shefali Bishnoi** | Security system: Intrusion detection, code verification, door control       |
| **Juhi Sahni**      | Fire detection: Flame sensing, emergency protocol, fire alarm management    |
| **Saniya Prakash**  | Rainwater system: Rain + tank sensors, valve control, adaptive thresholds   |
| **Manvitha Reddy**  | Smart lighting: Motion sensing, energy-efficient light control              |

---

## 🖥️ Getting Started

1. Connect all components as per the provided circuit diagram.
2. Upload the Arduino code to your UNO/Mega.
3. Open Serial Monitor at 9600 baud to interact with access code system and debug outputs.
4. Power on and test each module independently and in integration.

---

