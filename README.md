# 🛡️ Entry Monitoring System with Metal Detection

This project is a smart entry monitoring system using **NodeMCU (ESP8266)** that:

- 👥 Counts people entering and exiting
- 🧲 Detects metallic objects
- 🖥️ Displays data on an LCD
- 📱 Sends real-time updates to the Blynk IoT app
- 🔊 Alerts via buzzer and LED

---

## 📌 Features

- ✅ **IR Sensors** detect entry and exit
- ✅ **Metal Sensor** triggers alerts for metallic objects
- ✅ **LCD I2C Display** shows live count and alerts
- ✅ **Blynk Integration** for remote monitoring via mobile app
- ✅ **Buzzer and LED** give real-time physical feedback

---

## 🧰 Hardware Used

| Component               | Quantity |
|------------------------|----------|
| NodeMCU (ESP8266)      | 1        |
| IR Sensors             | 2        |
| Inductive Metal Sensor | 1        |
| Buzzer                 | 1        |
| LED                    | 1        |
| LCD 16x2 with I2C      | 1        |
| Jumper Wires           | As needed |
| Breadboard / PCB       | 1        |

---

## 📱 Blynk Setup

- Use the [Blynk IoT platform](https://blynk.cloud/)
- Create 2 virtual pins:
  - `V0` – People count
  - `V1` – Metal detection status (1 = Detected, 0 = Clear)
- Replace the placeholders in the code:
  ```cpp
  #define BLYNK_TEMPLATE_ID "YourTemplateID"
  #define BLYNK_TEMPLATE_NAME "YourProjectName"
  #define BLYNK_AUTH_TOKEN "YourAuthToken"
