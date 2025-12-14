# 👁️ TRINETRA - Advanced AI Surveillance System

![Python](https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge&logo=python)
![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-green?style=for-the-badge&logo=opencv)
![YOLOv8](https://img.shields.io/badge/YOLOv8-Object%20Detection-orange?style=for-the-badge)
![FaceID](https://img.shields.io/badge/Face%20Recognition-Security-red?style=for-the-badge)

**Trinetra** is a Next-Gen Smart Surveillance System designed to automate threat detection. Unlike traditional CCTV that only records, Trinetra **analyzes, identifies, and alerts** in real-time.

It integrates **Weapon Detection**, **Criminal Identification**, and **SOS Gesture Recognition** into a unified Cyberpunk-style Dashboard.

---

## 🚀 Key Features

### 1. 🔫 Real-time Weapon Detection
- Uses **YOLOv8 (Small)** model to detect threats like Knives, Guns, Scissors, etc.
- **Accuracy:** Optimized for long-range detection (Resized processing).
- **Instant Alert:** Triggers a siren and sends a Telegram notification immediately.

### 2. 👤 Criminal Identification (Face Recognition)
- Matches faces against a `wanted_criminals` database.
- **Smart Feedback:**
  - 🟢 **Green Box:** Recognized as "Citizen" (Safe).
  - 🔴 **Red Box:** Match Found -> "WANTED CRIMINAL" (Alert Triggered).
- Uses **High-Accuracy Encoding** with strict tolerance logic.

### 3. ✋ SOS Gesture Control (Dead Man's Switch)
- Uses **MediaPipe Hand Tracking**.
- **Logic:** If a user holds a **Closed Fist (Mutthi)** for **5 Seconds**, the system triggers a Silent Distress Signal.
- Useful for situations where speaking is not possible.

### 4. ⚡ Instant Alerts System
- **Siren:** Plays a loud alarm locally (`siren.mp3`).
- **Telegram Bot:** Sends a photo proof + location + threat type to the authorities instantly.
- **Database Logging:** Records every incident in an SQLite database for future forensics.

---

## 🛠️ Tech Stack

* **Core:** Python 3.11
* **AI/ML:** Ultralytics YOLOv8, Face_Recognition (Dlib), MediaPipe
* **Backend:** Flask (Python Web Framework)
* **Frontend:** HTML5, CSS3 (Cyberpunk Theme), JavaScript (Fetch API)
* **Database:** SQLite3
* **Hardware Support:** Works on Standard Laptops (Optimized for CPU) & CCTV Feeds.

---

## 📸 Screenshots

*(You can add screenshots of your dashboard here later)*

---

## ⚙️ Installation & Setup

### Prerequisites
- Python 3.10 or 3.11
- A Webcam
- Visual C++ Redistributable (for Windows)

### 1. Clone the Repository
```bash
git clone [https://github.com/your-username/trinetra.git](https://github.com/your-username/trinetra.git)
cd trinetra