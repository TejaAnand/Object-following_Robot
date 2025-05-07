# 🤖 Object Following Robot

## 📌 Overview
The **Object Following Robot** is a smart robotic system designed to detect and follow humans or objects using a combination of **ultrasonic** and **infrared (IR) sensors**. It's ideal for hospital delivery bots, luggage carriers in malls, or future defense robots.

---

## 🔧 Hardware Components

| Component                   | Quantity | Description                                             |
|-----------------------------|----------|---------------------------------------------------------|
| Arduino UNO                 | 1        | Microcontroller board acting as the brain               |
| L293D Motor Driver Shield   | 1        | Controls motor speed and direction                      |
| IR Sensors                  | 2        | Detect lateral object proximity                         |
| Ultrasonic Sensor (HC-SR04)| 1        | Detects frontal obstacles and object distance           |
| SG90 Servo Motor            | 1        | Rotates the ultrasonic sensor for scanning              |
| DC Geared Motors            | 4        | Drive the robot                                         |
| Wheels                      | 4        | Enable movement                                         |
| Robot Chassis               | 1        | Frame to hold all components                           |
| Jumper Wires                | —        | Used for electrical connections                         |
| 18650 Rechargeable Batteries| 2+       | Power supply                                            |
| Switch                      | 1        | Turns the robot ON/OFF                                 |
| Tools                       | Various  | Soldering kit, screwdrivers, etc.                       |

---

## 💡 Features

- 🧍 Human/Object following within ~4 meters
- 🚧 Obstacle detection and avoidance
- 🤖 Arduino-based real-time control
- 🔌 Battery-powered and mobile

---

## 🛠️ Working Principle

The robot uses:
- **Ultrasonic sensor** to measure distance and detect frontal obstacles.
- **IR sensors** to detect side proximity and help guide turns.
- **Motor driver (L293D)** to control motor direction/speed based on sensor input.
- **Servo motor** to rotate the ultrasonic sensor for a wider scan.

All logic is handled by the **Arduino UNO**.

---

## 📂 File Structure

```yaml
object-following-robot/
├── object_following_robot.ino    # Arduino source code
├── slides_.pdf                   # Project documentation (overview, working, block diagram)
├── README.md                     # Full project description and setup instructions
└── requirements.txt              # Optional, for Python-based versions (not used in Arduino)


---

## 🚀 Setup & Usage

1. **Assemble Hardware:** Connect components as shown in `slides_.pdf`.
2. **Upload Code:** Open `object_following_robot.ino` in Arduino IDE and upload to the board.
3. **Power On:** Connect batteries and switch on.
4. **Operation:** Place an object or walk in front of the robot. It will follow and avoid obstacles.

---

## 📈 Result

- Robot follows the user or object reliably
- Maintains safe distance using ultrasonic sensing
- Avoids collisions and changes direction based on IR inputs

---

## 🔭 Future Enhancements

- Bluetooth/Wi-Fi remote control
- Object recognition using camera & AI
- Voice command support
- Better power management

---

## 🧑‍💻 Authors
- P.Teja Anand

---
