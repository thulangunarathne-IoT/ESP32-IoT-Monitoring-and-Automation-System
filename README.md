# ESP32-IoT-Monitoring-and-Automation-System
Industrial IoT monitoring and automation system using ESP32, MQTT, Node-RED, sensors, and relay based load control.
The system provides real-time monitoring of environmental conditions, gas levels, electrical current/power consumption, Wi-Fi strength, Device status motion detection, light detection, automated light control, and manual load & alarm control through a Node-RED dashboard.

🚀 Features
-
🌡️ Temperature and humidity monitoring using DHT22

💨 Gas level monitoring using MQ-2

🚨 Gas warning and danger alarm

🚶 PIR-based motion detection

💡 Dark/Bright environment detection using LDR

💡 Automatic light control using relay

🎛️ Manual load and alarm control from the dashboard

🎛️ load and alarm status monitoring

⚡ AC current and power monitoring using ACS712

🔋 Energy consumption monitoring (kWh)

📡 MQTT-based communication

📊 Real-time Node-RED dashboard

📶 ESP32 device status monitoring

📶 Wi-Fi strength monitoring

🔔 Audible gas alarm using a buzzer


🏗️ System Architecture
-
Sensors:
│ DHT22 │
│ MQ-2 │
│ PIR │
│ LDR │
│ ACS712 │

ESP32:
│ Sensor Processing │
│ Automation Logic │
│ Relay Control │
│ Wi-Fi / MQTT │

MQTT Broker: | Hive MQ |

Node-RED:
│ Monitoring │
│ Dashboard │
│ Manual Control │
│ Alarm │

⚙️ Automation Logic
-
Automatic Lighting:

The system can automatically control a connected light based on environmental conditions:

Dark + Motion Detected
↓
ESP32 detects conditions
↓
Relay ON
↓
Light ON

Manual Load and alarm Control:

The Node-RED dashboard provides manual control of the connected load and alarm.

User
↓
Node-RED Dashboard
↓
MQTT
↓
ESP32
↓
Relay
↓
Load/Alarm

Manual control allows the user to override or directly control the connected load and alarm from the dashboard.

📊 Monitoring
-
The Node-RED dashboard provides real-time information including:

Temperature

Humidity

Gas level

Gas status

Motion status

Dark/Bright status

Current

Power

Energy consumption

Device status

Wi-Fi strength

Load status

Gas alarm status

🚨 Gas Detection
-
The MQ-2 sensor is used to monitor gas levels.
The ESP32 processes the sensor reading and activates an audible alarm when the gas level reaches the configured warning/danger thresholds.

⚡ Energy Monitoring
-
An ACS712 current sensor is used to measure the current consumed by the connected AC load.
The ESP32 sends the data through MQTT for visualization on the Node-RED dashboard and Node-RED calculates electrical power and energy consumption.

🧰 Hardware
-
ESP32 development board

DHT22 temperature/humidity sensor

MQ-2 gas sensor

PIR motion sensor

ACS712 current sensor

LDR sensor

Relay modules

Active buzzer

AC load

5 V DC power supply

PVC enclosure

Perfboard

Connecting wires and supporting components

💻 Software & Technologies
-
Arduino IDE

ESP32

C/C++

MQTT.

Node-RED

Mosquitto/HiveMQ-compatible MQTT communication

Wi-Fi

JSON/MQTT messaging

📡 Communication
-
The ESP32 communicates with the Node-RED system using the MQTT protocol.

Example MQTT topics used in the project include:

factory/room1/device/status

factory/room101/motion

MQTT provides lightweight and efficient communication between the ESP32 and the monitoring/control system.

🎯 Project Objectives
-
The main objectives of this project are:

Monitor multiple sensors using an ESP32

Send real-time sensor information using MQTT

Visualize data through a Node-RED dashboard

Automate electrical loads based on sensor conditions

Provide manual remote load control

Monitor electrical current, power, and energy consumption

Implement gas detection and alarm functionality

Demonstrate practical Industrial IoT concepts

🔧 Skills Demonstrated
-
This project demonstrates practical experience in:

Embedded Systems

ESP32 Programming
.
Arduino Programming

IoT Development

MQTT Communication

Node-RED

Sensor Integration

Relay Automation

AC Load Control

Energy Monitoring

Wi-Fi Communication

Troubleshooting Electronics

Automation Logic

📌 Project Status
-
Completed ✅

This project was designed, assembled, programmed, tested, and integrated as a complete ESP32-based IoT monitoring and automation system.

🔮 Future Improvements
-
Possible future improvements include:

ESP32-CAM integration

Cloud data storage

Mobile application

Historical data visualization

Database integration

Multiple ESP32 nodes

Remote notifications

Advanced energy analytics

Improved gas concentration calibration

User authentication and security

👨‍💻 Author
-
Thulan Gunarathne

Electronic & Communication Engineer|
Embedded Systems & IoT Developer

GitHub: thulangunarathne-iot
