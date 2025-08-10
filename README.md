# Illegal-Parking-Monitoring-System-using-Computer-Vision
This project is an automated illegal parking detection and reporting system designed to assist local authorities in enforcing parking regulations efficiently.
The system leverages computer vision, license plate recognition, and real-time alerting to replace slow and inefficient manual monitoring.

## 📍 Deployment Context
- **Location:** Barangay Cembo, Taguig City — Acacia Street (frequent illegal parking site)  
- **Camera Setup:** IP camera with integrated computer vision module  
- **Target Vehicles:** Light vehicles (motorcycles) & 4-wheeled vehicles (cars, vans, trucks)

## 🔹 Features
- **Vehicle Detection & Classification**  
  - Detects vehicles in a 15-meter range using YOLO-based object detection  
  - Differentiates between light vehicles and 4-wheeled vehicles  
- **Parking Duration Tracking**  
  - Light vehicles monitored over a 5-minute window  
  - 4-wheeled vehicles trigger:  
    a. 1-minute warning (voice alert)  
    b. 3-minute license plate scan and violation logging  
- **License Plate Recognition**  
  - 100% accuracy up to 10 meters  
  - Beyond range → marked as Unknown  
- **Automated Alerts & Notifications**  
  - Voice announcements for onsite warnings  
  - SMS alerts via Twilio to local officials for violations  
  - Video recording (2 minutes) for evidence  
- **Live Monitoring Interface**  
  - Real-time feed accessible via a local web server  
  - Recorded footage and violation logs stored locally  

## 📊 Performance Results
- Vehicle detection & violation identification: **100% accuracy** (≤15m)  
- Plate recognition accuracy: **100%** (≤10m)  
- Warning, SMS, & recording automation: **100% success rate**  

## 🛠️ Tech Stack
- **Programming Language:** Python  
- **Frameworks/Libraries:** OpenCV, YOLO (Ultralytics), EasyOCR / PaddleOCR (for LPR)  
- **Database/Logging:** Local storage with structured text log files  
- **Alert System:** Twilio API (SMS), Local audio output for warnings  
- **Interface:** Flask/Tkinter (custom live feed viewer)  
- **Hardware:** IP Camera, Local Server/PC  

## 🚀 Potential Applications
- Urban traffic management in high-density parking areas  
- Barangay-level and city-wide deployment  
- Integration with municipal ticketing systems  

## 📄 License
This project is licensed under the MIT License – see the LICENSE file for details.
