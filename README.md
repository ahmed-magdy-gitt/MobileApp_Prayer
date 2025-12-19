# 🕌 Athan Mate: Prayer Times & Qibla Finder

![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)
![Retrofit](https://img.shields.io/badge/Retrofit-Networking-cc0000?style=for-the-badge)
![Sensors](https://img.shields.io/badge/Sensors-Compass_%26_GPS-orange?style=for-the-badge)

## 📱 Project Overview
**Athan Mate** is a comprehensive Islamic utility application built with **Native Android (Kotlin)**. It serves as a daily spiritual companion, combining real-time data fetching with complex device sensor integration.

The app features a precision-engineered **Qibla Compass** that calculates the direction of the Kaaba based on the user's geolocations, alongside accurate prayer timings fetched dynamically via REST APIs.

## ✨ Key Features

### 🕋 Smart Qibla Compass (The Technical Core)
* **Mathematical Precision:** Implements complex Trigonometric formulas (Haversine/Great Circle) using `atan2`, `sin`, and `cos` to calculate the exact bearing to Makkah.
* **Sensor Fusion:** Utilizes the device's **Magnetometer** and **Accelerometer** to create a responsive, real-time rotating compass UI.
* **GPS Integration:** Uses `FusedLocationProviderClient` to get the user's precise coordinates (Latitude/Longitude).

### ⏳ Real-Time Prayer Times
* **API Integration:** Connects to the **Aladhan API** using **Retrofit** & **Gson** to fetch timings for Fajr, Dhuhr, Asr, Maghrib, and Isha.
* **Dynamic Parsing:** Handles JSON responses efficiently to display formatted time strings.

### 📿 Digital Azkar
* **Interactive List:** A clean interface allowing users to toggle through daily supplications (Azkar).
* **State Management:** Simple cycling logic to display the next Zikr upon interaction.

---

## 🛠️ Tech Stack
This project demonstrates proficiency in dealing with Hardware Sensors and Networking:

<p align="left">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=android,kotlin,java,idea,git" />
  </a>
</p>

| Component | Technology |
| :--- | :--- |
| **Language** | Kotlin |
| **Networking** | Retrofit 2 & Gson Converter |
| **Location Services** | Google Play Services (FusedLocation) |
| **Hardware** | Android SensorManager (Orientation/Magnetic) |
| **UI/UX** | ViewBinding, Animations, XML |

## 📸 Screenshots

| Prayer Times (Home) | Qibla Compass | Azkar Section |
| :---: | :---: | :---: |
| ![WhatsApp Image 2025-12-19 at 11 24 59_3d612294](https://github.com/user-attachments/assets/19983419-576b-45dd-a5a9-d001f89696fe)|![WhatsApp Image 2025-12-19 at 11 24 59_93ff6d30](https://github.com/user-attachments/assets/8d64fe60-c9b6-4c83-9f9c-31bdbfb18385)| ![WhatsApp Image 2025-12-19 at 11 24 59_840c6bbc](https://github.com/user-attachments/assets/7e128231-f24f-492a-9d68-9bf424f55ee5)|

> *Note: Ensure your device has GPS enabled for the Qibla feature to function correctly.*

## 🚀 How to Run
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/ahmed-magdy-gitt/Athan-Mate.git](https://github.com/ahmed-magdy-gitt/Athan-Mate.git)
    ```
2.  **Permissions:**
    * The app will request `ACCESS_FINE_LOCATION` to calculate Qibla direction.
3.  **Build & Run:**
    * Open in Android Studio and run on a physical device (Emulators may not simulate sensors correctly).

---
*Developed by Ahmed Magdy | 2025*
*Android Developer Portfolio*
