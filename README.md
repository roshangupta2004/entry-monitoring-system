# 🛡️ Entry Monitoring System with Metal Detection

This project is a smart entry monitoring solution using **NodeMCU (ESP8266)** that tracks:
- 👥 Number of people entering/exiting
- 🧲 Presence of metallic objects
- 📱 Real-time monitoring via Blynk IoT app
- 🖥️ LCD display for on-site feedback
- 🔊 Alerts via buzzer and LED

---

## 📌 Features

- ✅ **IR Sensors** to detect entry and exit events
- ✅ **Inductive Metal Sensor** to detect if someone is carrying metal
- ✅ **Blynk Dashboard** to view people count and metal detection status remotely
- ✅ **LCD I2C Display** to show live count and status
- ✅ **Buzzer + LED** feedback for security alerts

---

## 🧰 Hardware Used

| Component           | Quantity |
|---------------------|----------|
| NodeMCU (ESP8266)   | 1        |
| IR Sensors          | 2        |
| Inductive Metal Sensor | 1     |
| Buzzer              | 1        |
| LED                 | 1        |
| LCD 16x2 with I2C   | 1        |
| Jumper Wires        | As needed |
| Breadboard / PCB    | 1        |

---

## 📱 Blynk Setup

- Use [Blynk IoT Platform](https://blynk.cloud/)
- Create 2 virtual pins:
  - `V0`: People Count
  - `V1`: Metal Detection Status (1 = detected, 0 = clear)
- Set `BLYNK_TEMPLATE_ID`, `BLYNK_TEMPLATE_NAME`, and `BLYNK_AUTH_TOKEN` in the code.

---

## 📸 Preview

| Live LCD View | Blynk Dashboard |
|---------------|-----------------|
| ![LCD](assets/lcd-preview.jpg) | ![Blynk](assets/blynk-preview.jpg) |

---

## 🧠 How It Works

- **Entry IR Sensor (D4)**: Increments people count
- **Exit IR Sensor (D5)**: Decrements count
- **Metal Sensor (D3)**: Triggers alert if metallic object detected
- **Buzzer (D8)**: Beeps on events
- **LED (D7)**: Blinks to show entry/exit or alert

---

## 📂 File Structure

