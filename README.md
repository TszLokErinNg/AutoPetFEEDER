# AutoPetFEEDER 🐾

An IoT-based solution designed to automate pet feeding and hydration while providing remote monitoring and multi-pet management.

## 📌 Project Overview
Pet owners often struggle to maintain consistent feeding schedules and manage different dietary needs for multiple pets. The **AutoPetFEEDER** addresses these challenges by utilizing IoT technology to provide a versatile, cloud-integrated system.

Unlike traditional feeders, this system supports:
* **Multi-Pet Identification:** Uses RFID to distinguish between different pets.
* **Real-time Monitoring:** Infrared and ultrasonic sensors monitor food and water levels.
* **Cloud Integration:** Remote control via MQTT and automated restocking capabilities.
* **Cost-Effective Design:** Built using accessible components like ESP32/ESP8266.

## 🚀 Key Features
- **RFID-Based Recognition:** Only dispenses specific food types for identified pets.
- **Inventory Management:** Tracks food/water levels and notifies the owner or triggers restocking via the cloud.
- **Remote Feeding:** Manual feeding override through a web interface or mobile app using the MQTT protocol.
- **Smart Hydration:** Monitoring system to ensure fresh water is always available.

## 🛠️ System Architecture
The project integrates hardware sensors with a cloud-based backend to create a seamless loop of data and action.

1.  **Sensing Layer:** * RFID Reader (MFRC522) for pet ID.
    * Ultrasonic Sensors for food storage levels.
    * Infrared/Water Level sensors for hydration tracking.
2.  **Control Layer:** * Microcontroller (ESP series) processes sensor data and controls servo motors for dispensing.
3.  **Communication Layer:** * MQTT protocol for low-latency communication between the device and the cloud.
4.  **Application Layer:** * Dashboard for monitoring pet activity and inventory status.

## 🔧 Hardware Requirements
- Microcontroller (e.g., ESP32 or ESP8266)
- RFID RC522 Module + Tags
- HC-SR04 Ultrasonic Sensor
- Servo Motors (for dispensing mechanism)
- IR Sensors / Water Level Sensor
- Power Supply (5V/12V depending on motors)

## 💻 Software & Libraries
- **Language:** C++/Arduino
- **Protocols:** MQTT, Wi-Fi
- **Key Libraries:** - `PubSubClient` (for MQTT)
  - `MFRC522` (for RFID)
  - `Servo` (for motor control)

## 📂 Repository Structure
* `Code/`: Contains the firmware for the microcontroller.
* `Documentation/`: Technical reports and diagrams.
* `Hardware/`: Circuit diagrams and 3D design files (if applicable).

## 📝 Future Scope
- Integration with AI for pet health behavioral analysis.
- Weight sensor integration for precise caloric intake tracking.
- Mobile application for iOS and Android.

## 🔗 Original Link
Find the full source code and documentation here: [AutoPetFEEDER Demonstration] (https://youtu.be/c0YBG-16054)
