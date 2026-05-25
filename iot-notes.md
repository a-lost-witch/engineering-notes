# 1. What is IoT?
IoT = Internet of Things

# 2. What are some Examples of IOT?
- Alexa
- Smart lights
- CCTV cameras

# 3. What is the architecture of IOT?  
Sensor
   ↓
Controller
   ↓
Internet/Wi-Fi
   ↓
Cloud Server
   ↓
Mobile App / User
   ↓
Actuator

# 4. Explain the components of IOT.
## - Sensors / Input Devices

Sensors collect data from the physical world.

Examples:
- Temperature sensor
- Humidity sensor
- Motion sensor
- Camera
- Microphone

Example:
A smart AC uses a temperature sensor to measure room temperature.

---

## - Controller / Processor

The controller acts as the brain of the IoT system.

Functions:
- Processes sensor data
- Makes decisions
- Sends commands

Examples:
- Arduino
- ESP32
- Raspberry Pi
- Microcontrollers

Example Logic:

IF temperature > 30°C  
THEN turn ON AC

---

# - Connectivity / Communication

IoT devices communicate using networks.

Communication methods:
- Wi-Fi
- Bluetooth
- Zigbee
- LoRa
- Ethernet
- 4G/5G

Purpose:
- Send data
- Receive commands
- Connect to cloud servers

---

## - Cloud / Server

The cloud stores and processes IoT data.

Functions:
- Data storage
- Data analysis
- Remote access
- AI processing
- Sending commands

Examples:
- AWS IoT
- Google Cloud IoT
- Microsoft Azure IoT

Physical Meaning:
The cloud is actually large data centers containing servers and storage systems.

---

## - Application / User Interface

The user interacts with the IoT system using applications.

Examples:
- Mobile apps
- Web dashboards
- Alexa voice interface
- Smartwatch apps

Functions:
- Monitor devices
- Control devices
- View data

---

# - Actuator / Output Device

Actuators perform physical actions.

Examples:
- Relay
- Motor
- Smart bulb
- Door lock
- Buzzer

Example:
A smart bulb receives a command and turns ON.

---

## Example: Alexa Smart Light System

User says:
"Alexa, turn on the light"

Process:

Voice Input
↓
Microphone captures sound
↓
Data sent through Wi-Fi
↓
Cloud server processes command
↓
Command sent to smart bulb
↓
Bulb controller activates circuit
↓
Light turns ON

# 5. What are the Technologies Used in IoT?

- Electronics
- Embedded Systems
- Sensors
- Networking
- Cloud Computing
- Software
- Automation
- Data Analytics
- Artificial Intelligence

# 6. Where is Data Stored in IoT?

In IoT (Internet of Things), data is usually stored in:

1. Cloud Servers (e.g AWS Cloud, Google Cloud, Microsoft Azure)
2. Local Storage (e.g. A CCTV camera may store video directly on an SD card)
3. Edge Devices (data processed and stored near the device. e.g. A factory machine analyzes sensor data locally using an industrial controller for  Faster response, Lower internet usage, Reduced cloud load)
4. Databases inside Data Centers (e.g. SQL)

# 7. What is Data represented with?
Data stored as binary bits are represented physically using:
- voltage levels
- electric charge
- magnetic orientation
- transistor states
- light pulses

# 8. What is SSD?
SSD is solid state device. Inside SSD,
Electrons trapped      → 0 binary state
Electrons absent       → 1 binary state
This storage remains even after power OFF. This is because SSD uses Flash memory (Floating-Gate MOSFET)

# 9. Why do electrons stay trapped in Floating gate MOSFET?
A flash-memory transistor has an extra insulated region called a floating gate. This insulating material (oxide layer) acts like a wall. Thus data stays non volatile.

# 10. What is Edge Computing?
Edge Computing is a method where data is processed near the device itself instead of sending everything to a distant cloud server.

Instead of:
Device → Internet → Cloud → Processing
Edge computing does:
Device → Local Processing → Immediate Result

# 11. What is an Actuator?

An actuator is an output device that converts electrical signals into physical action. It converts electrical, pneumatic or hydraulic input to force, torque, or displacement. E.g. Servo Motor

## Actuators can:
- Move objects
- Rotate motors
- Open valves
- Switch relays
- Produce sound
- Turn lights ON/OFF

# 12. What are the types of motion in actuator?
Actuators can be categorized into linear (Forward/backward, Up/down, Push/pullor) and rotary based on their movement type.

## Examples of Linear Actuators:
a) Solenoid
b) Hydraulic Cylinder
c) Pneumatic Cylinder

---
 ## Examples of Rotary Actuators:
a) DC Motor
b) Servo Motor
c) Stepper Motor

# 13. Differentiate between DC motor, servo motor and stepper motor.

# Key Differences

| Feature | DC Motor | Stepper Motor | Servo Motor |
|----------|-----------|---------------|--------------|
| Control Mechanism | Continuous rotation; speed depends on voltage | Open-loop; moves in exact "steps" based on electrical pulses | Closed-loop; uses built-in feedback to hit exact angles |
| Accuracy & Precision | Low. Cannot hold an exact position | Very High. Loses accuracy only if a step is skipped | Extremely High. Actively corrects position if forced out of place |
| Speed | High RPM | Best at low to medium speeds | High speed with maintained torque |
| Holding Torque | Poor when powered off | Excellent holding torque | Excellent active holding |
