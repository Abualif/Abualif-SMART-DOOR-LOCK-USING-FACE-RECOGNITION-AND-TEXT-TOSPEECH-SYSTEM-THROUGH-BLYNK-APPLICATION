# Smart Door Lock with Face Recognition, Blynk, and Text-to-Speech

This project is an **IoT-based Smart Door Lock** that uses an ESP32-CAM to perform **local face recognition**, **control a solenoid lock**, and provide **real-time monitoring and notifications** via the **Blynk** application and a web dashboard.

## 📋 Overview

The system improves door security by replacing conventional keys with face recognition. Registered faces are stored locally, and the door unlocks only when a registered face is detected. It also provides audio feedback through browser-based **text-to-speech**, live camera streaming, and remote control via smartphone.

## 🔧 Features

- ✅ Local face detection and recognition on ESP32-CAM
- ✅ Real-time video streaming on web dashboard and Blynk
- ✅ Automatic door unlocking with solenoid lock and relay
- ✅ Manual control and notifications via Blynk mobile app
- ✅ Audio notification (text-to-speech) in browser when door opens
- ✅ Public remote access enabled with VPS and Fast Reverse Proxy (FRP)

---

## 🖥️ System Components

- **ESP32-CAM**: Main controller for face recognition, streaming, and WebSocket server
- **Relay module**: Controls the solenoid lock
- **Solenoid lock**: Electromechanical actuator for locking/unlocking the door
- **VPS (Virtual Private Server)**: Hosts FRP server for public access
- **FRP (Fast Reverse Proxy)**: Enables stable internet access from outside the local network
- **Blynk app**: Mobile app for remote monitoring, control, and notifications
- **Web dashboard**: For face registration, streaming, and control

---

## 🚀 How It Works

1️⃣ User face is registered through the web dashboard and stored locally on ESP32-CAM.  
2️⃣ ESP32-CAM continuously monitors and detects faces through its camera.  
3️⃣ If a registered face is detected, ESP32-CAM sends a signal via relay to unlock the solenoid lock.  
4️⃣ The system sends a real-time notification to the user via Blynk and plays an audio confirmation (text-to-speech) in the browser.  
5️⃣ Video streaming and manual control are accessible via the dashboard or Blynk app.  
6️⃣ VPS and FRP make the dashboard and ESP32-CAM accessible remotely.

---

## 🌐 Technologies Used

- ESP32-CAM with Arduino IDE
- WebSocket & HTTP server
- Blynk IoT platform
- VPS + FRP (Fast Reverse Proxy) for public access
- HTML/CSS/JavaScript for web dashboard
- Browser Text-to-Speech API

---

## 📖 Usage

1. Flash the ESP32-CAM with the provided firmware.
2. Set up your VPS and configure FRP for tunneling.
3. Deploy the web dashboard files to your server.
4. Connect ESP32-CAM to WiFi, start the server, and register user faces.
5. Use the dashboard or Blynk app to monitor, control, and receive notifications.

---

## 📄 Authors & License

Developed by **Abu Alif Raharjo** as a final project at Universitas Gadjah Mada, 2025.  
License: MIT (or specify another license if applicable).
