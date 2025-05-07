# 🤖 Object Following Robot

## 📌 Overview
The **Object Following Robot** is a smart robotic system designed to detect and follow humans or objects using a combination of **ultrasonic** and **infrared (IR) sensors**. It's ideal for applications like **hospital delivery bots**, **luggage carriers in malls**, and **defense robots**.

---

## 🔧 Hardware Components

| Component                     | Quantity | Description                                               |
|-------------------------------|----------|-----------------------------------------------------------|
| Arduino UNO                   | 1        | Microcontroller board, the brain of the robot             |
| L293D Motor Driver Shield     | 1        | Controls motor speed and direction                        |
| IR Sensors                    | 2        | Detect lateral proximity of objects                       |
| Ultrasonic Sensor (HC-SR04)    | 1        | Measures distance and detects frontal obstacles           |
| SG90 Servo Motor              | 1        | Rotates the ultrasonic sensor for scanning                |
| DC Geared Motors              | 4        | Drives the robot's movement                               |
| Wheels                        | 4        | Enables movement of the robot                             |
| Robot Chassis                 | 1        | Frame to mount all components                             |
| Jumper Wires                  | —        | For connecting the components                             |
| 18650 Rechargeable Batteries   | 2+       | Power supply for the robot                                |
| Switch                        | 1        | Turns the robot on/off                                    |
| Tools                         | Various  | Soldering kit, screwdrivers, etc.                         |

---

## 💡 Features

- 🧍 **Human/Object Following:** Detects and follows humans or objects within ~4 meters.
- 🚧 **Obstacle Detection & Avoidance:** Prevents collisions using ultrasonic and IR sensors.
- 🤖 **Real-Time Control:** Arduino-based system for smooth operation.
- 🔌 **Mobile & Battery-Powered:** Provides flexibility and mobility for various uses.

---

## 🛠️ Working Principle

- **Ultrasonic Sensor (HC-SR04):** Measures the distance to objects in front and helps the robot maintain a safe following distance.
- **IR Sensors:** Detect lateral proximity to objects and guide the robot’s turns.
- **L293D Motor Driver Shield:** Controls motor direction and speed based on sensor inputs, ensuring smooth movement and obstacle avoidance.
- **SG90 Servo Motor:** Rotates the ultrasonic sensor to scan in a wider range, improving the robot's ability to detect objects.
- The **Arduino UNO** microcontroller processes all sensor data and controls the robot’s movements in real-time.

---

## 📂 File Structure

```plaintext
object-following-robot/
├── object_following_robot.ino    # Arduino code for robot operation
├── slides_.pdf                   # Project documentation (overview, working, block diagram)
├── README.md                     # Full project description and setup instructions
└── requirements.txt              # Optional, for Python-based versions (not used in Arduino)

```
🚀 Setup & Usage

Assemble Hardware:
Follow the wiring diagram in the slides_.pdf for connecting all components.
Upload Code:
Open the object_following_robot.ino file in the Arduino IDE.
Upload the code to your Arduino UNO board.
Power On:
Connect the 18650 rechargeable batteries to the power input and turn the switch on.
Operation:
Place an object or walk in front of the robot. It will autonomously follow the object and avoid obstacles in its path.
📈 Result

Autonomous Following: The robot successfully follows a person or object.
Safe Distance Maintenance: The ultrasonic sensor ensures the robot maintains a safe following distance.
Obstacle Avoidance: The robot detects and avoids obstacles using the IR sensors and changes direction as necessary.
🔭 Future Enhancements

Remote Control: Add Bluetooth or Wi-Fi functionality to control the robot remotely.
Object Recognition: Implement a camera and AI for enhanced object recognition capabilities.
Voice Command Integration: Enable voice commands to control the robot.
Improved Power Management: Implement better power-saving techniques to extend battery life.
🧑‍💻 Author

P. Teja Anand
