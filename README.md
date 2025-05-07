# 🤖 Object Following Robot

## 📌 Overview
The **Object Following Robot** is an intelligent robotic system designed to detect and follow a human or object using a combination of **ultrasonic** and **IR sensors**. It automates movement based on proximity sensing and is ideal for applications in **medical assistance**, **shopping**, and **military support**.

---

## 🔧 Hardware Components

| Component                | Quantity | Description                                           |
|--------------------------|----------|-------------------------------------------------------|
| Arduino UNO              | 1        | Main microcontroller board                           |
| L293D Motor Driver Shield| 1        | Motor control module                                 |
| IR Sensors               | 2        | Infrared sensors for side/object detection           |
| Ultrasonic Sensor (HC-SR04) | 1    | For measuring distance and obstacle avoidance        |
| SG90 Servo Motor         | 1        | For directional sensor mounting                      |
| DC Geared Motors         | 4        | Drive the robot’s wheels                             |
| Wheels                   | 4        | For mobility                                          |
| Robot Chassis            | 1        | Structure to hold components                         |
| Jumper Wires             | As needed| Connections between components                       |
| 18650 Rechargeable Batteries | 2+   | Power supply                                          |
| Battery Holder & Switch  | 1 each   | To manage power on/off                               |
| Tools                    | -        | Soldering kit, screwdriver, wire cutter, etc.        |

---

## 💡 Features
- Follows a person or object within ~4 meters
- Avoids obstacles using ultrasonic detection
- Uses IR for lateral object tracking
- Controlled by Arduino and motor driver

---

## 🛠️ Working Principle

- **Ultrasonic sensor** detects distance and adjusts movement forward or backward.
- **IR sensors** detect lateral displacement and guide left or right turns.
- **Servo motor** can help rotate ultrasonic sensor for wider detection.
- All components are controlled via Arduino UNO using PWM and digital I/O pins.

---

## 🚀 Setup & Usage

1. **Wiring:** Connect all hardware as shown in the `Object-Following_Robot.pdf`.
2. **Upload Code:** Flash `Object-Following_Robot.ino` to Arduino using the Arduino IDE.
3. **Power Up:** Insert batteries and turn on the switch.
4. **Test:** Place an object/human within range. The robot should follow it.

---

## 📈 Result

The robot can:
- Accurately follow a human/object in real-time
- Maintain a set distance (within 4 meters)
- Avoid obstacles on its path

---

## 🔭 Future Improvements

- Add wireless control via Bluetooth/Wi-Fi
- Add camera for object recognition
- Upgrade motors and chassis for outdoor use
- Implement real-time tracking via mobile app

---

## 🧑‍💻 Authors
- P.Teja Anand

---
