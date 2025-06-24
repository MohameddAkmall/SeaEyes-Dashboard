# Sea Eyes – Smart Vessel Collision Avoidance System

**Sea Eyes** is a real-time Flutter mobile app designed to enhance maritime safety through intelligent vessel monitoring. It connects with a Raspberry Pi-based onboard system that gathers data from multiple sensors and streams it to the app using Firebase.

## 🌊 Overview

The app displays live data from the boat’s sensors on a modern dashboard interface. It helps users monitor their surroundings and avoid collisions by visualizing short-, mid-, and long-range zones.

## 🚢 Features

- **Real-Time Map Tracking**  
  Shows live GPS location of the boat and nearby vessels on a dynamic map.

- **Radar Visualization**  
  Semi-circular radar sweep using TfMini lidar sensor on servo motor.

- **Ultrasonic and Sonar Feedback**  
  Visual alert system for obstacles in the short-range zone.

- **Object Detection Integration** *(Coming Soon)*  
  Mid-range camera view with distance estimation.

- **Live Weather Forecast**  
  Dynamic weather screen with animated cards and time-based gradient backgrounds.

- **Danger Zone Alerts**  
  Notifications for orange and red zone proximity risks.

- **Firebase Realtime Database**  
  Cloud-based backend for syncing sensor data in real time.

## 📦 Tech Stack

- **Frontend:** Flutter (Dart)
- **Backend / Realtime Sync:** Firebase Realtime Database
- **Hardware Integration:** Raspberry Pi, GPS, TfMini, HC-SR04 Ultrasonic, Sonar
- **Data Visualization:** Custom radar UI, interactive map, weather cards


## 🔧 Setup

### Prerequisites

- Flutter SDK
- Firebase project setup (Realtime Database)
- Raspberry Pi with sensor firmware ready

### Steps

1. Clone the repo:
   ```bash
   git clone https://github.com/MohamedAkmall/sea-eyes.git
   cd sea-eyes
Install dependencies:

bash
Copy
Edit
flutter pub get
Configure Firebase:

Add google-services.json to /android/app

Set up Firebase Realtime Database structure (see example below)

Run the app:

bash
Copy
Edit
flutter run
🗂️ Firebase Data Structure (Example)
json
Copy
Edit
{
  "gps": {
    "lat": 31.123456,
    "lon": 29.987654
  },
  "ultrasonic": {
    "front": 40,
    "left": 30,
    "right": 45,
    "back": 50
  },
  "lidar": {
    "angle_0": 250,
    "angle_10": 240,
    ...
    "angle_180": 300
  }
}
📍 Project Status
✅ Mobile app
✅ GPS + radar visualization
✅ Firebase integration
🚧 Object detection + camera feed (Coming Soon)

👨‍💻 Author
Mohamed Akmal Samy 
Electronics and Communication Engineer
