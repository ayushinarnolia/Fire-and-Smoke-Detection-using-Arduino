# 🔥 Arduino-Based Smart Fire and Smoke Detection with AI Integration

This project presents an intelligent fire and smoke detection system using **Arduino Uno**, combining traditional sensors with **AI-based anomaly detection** for enhanced safety. The system delivers real-time alerts via a **buzzer**, **LCD display**, **voice output**, and **Telegram messages**, while also providing **live graphing** of sensor data.

## 📑 Abstract

An AI-enhanced fire and smoke detection system is developed using Arduino Uno with an MQ-2 smoke sensor, flame sensor, and a 16×2 LCD. Sensor data is analyzed in real time using an **Isolation Forest model** in Python. Upon detecting fire or smoke, the system triggers a buzzer, displays alerts, sends voice announcements, and delivers Telegram notifications. The hybrid approach significantly reduces false alarms and improves response time compared to traditional threshold-only systems.

## 🛠️ Components Used

- Arduino Uno
- MQ-2 Gas/Smoke Sensor
- Flame Sensor
- 16×2 I2C LCD Display
- Buzzer
- Breadboard & Jumper Wires
- USB Cable (for power & data)

## 💻 Software and Tools

- Arduino IDE (C/C++)
- Python (PySerial, Scikit-learn, Matplotlib, Pyttsx3, python-telegram-bot, Asyncio)
- Isolation Forest for anomaly detection
- Telegram Bot for remote alerts

## ⚙️ How It Works

1. Arduino reads values from the MQ-2 and flame sensors.
2. Basic threshold check triggers buzzer + LCD alert.
3. Sensor data is sent via serial to Python.
4. Python's Isolation Forest model checks for anomalies.
5. On anomaly/fire detection:
   - Voice alert is announced.
   - Telegram alert is sent.
   - Live graph is updated with Matplotlib.

## 📊 Performance Summary

| Metric                   | Result                         |
|--------------------------|--------------------------------|
| Smoke Detection Accuracy | ~93.3%                         |
| Flame Detection Accuracy | 100%                           |
| Avg Alert Delay          | < 2 seconds                    |
| Voice Alert Latency      | ~1.5 seconds                   |
| Telegram Alert Delay     | 2–4 seconds (network dependent)|
| False Positives          | 2 out of 50 test runs          |

## 📸 Highlights

- Real-time LCD and buzzer alerts
- AI-powered detection using Isolation Forest
- Voice output using text-to-speech
- Telegram notifications to user
- Live plotting of sensor values

## 📄 Research Paper

Read the full IEEE-style report here: **[IEEE_Report.pdf](./IEEE_Report.pdf)**

## 🚀 Future Enhancements

- Deploy deep learning via TensorFlow Lite
- Add more sensors (temperature, CO, humidity)
- Cloud dashboard and mobile app integration
- Use NodeMCU/ESP32 for wireless IoT capabilities

## 👩‍💻 Authors

- **Ayushi Narnolia** (23BAI0191)  
- Madhav Mendiratta (23BCB0092)  
- Shreya Gupta (23BAI0168)  
- Ankit Kumar (23BCB0131)  
- **Guide**: Prof. Debashish Dash (SENSE, VIT Vellore)

---

