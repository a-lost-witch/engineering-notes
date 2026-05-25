## 1. What is IoT?
IoT = Internet of Things

## 2. What are some Examples of IOT?
- Alexa
- Smart lights
- CCTV cameras

## 3. What is the architecture of IOT?  
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

## 4. Explain the components of IOT.
# - Sensors / Input Devices

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

# - Controller / Processor

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

# - Cloud / Server

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

# - Application / User Interface

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

# Example: Alexa Smart Light System

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

## 5. What are the Technologies Used in IoT?

- Electronics
- Embedded Systems
- Sensors
- Networking
- Cloud Computing
- Software
- Automation
- Data Analytics
- Artificial Intelligence

## 6. Where is Data Stored in IoT?

In IoT (Internet of Things), data is usually stored in:

1. Cloud Servers (e.g AWS Cloud, Google Cloud, Microsoft Azure)
2. Local Storage (e.g. A CCTV camera may store video directly on an SD card)
3. Edge Devices (data processed and stored near the device. e.g. A factory machine analyzes sensor data locally using an industrial controller for  Faster response, Lower internet usage, Reduced cloud load)
4. Databases inside Data Centers (e.g. SQL)

## 7. What is Data represented with?
Data stored as binary bits are represented physically using:
- voltage levels
- electric charge
- magnetic orientation
- transistor states
- light pulses

## 8. What is SSD?
SSD is solid state device. Inside SSD,
Electrons trapped      → 0 binary state
Electrons absent       → 1 binary state
This storage remains even after power OFF. This is because SSD uses Flash memory (Floating-Gate MOSFET)

## 9. Why do electrons stay trapped in Floating gate MOSFET?
A flash-memory transistor has an extra insulated region called a floating gate. This insulating material (oxide layer) acts like a wall. Thus data stays non volatile.
