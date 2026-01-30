# 📍 Simple Location Tracker App

## 📱 App Description

The **Simple Location Tracker App** is a basic Android mobile application that displays the user’s **live GPS location on a map**. It uses the device’s built-in location services to track movement and update the user’s position in real time. The app is designed to demonstrate how mobile devices interact with physical-world data such as GPS while maintaining simplicity and respecting user privacy.

The application consists of a **single screen** that shows a map with a marker indicating the user’s current location.

---

## 🛠 Features Implemented

* Runtime location permission request and handling
* Google Map displayed on screen
* Marker showing the user’s current GPS location
* Automatic location updates as the device moves
* Simple and clean single-screen UI

---

## 🔐 Permissions Used

The app requires the following permissions:

* `ACCESS_FINE_LOCATION` – Used to obtain precise GPS location
* `ACCESS_COARSE_LOCATION` – Used as a fallback for approximate location

Runtime permission requests are implemented to ensure the app does not crash when permission is denied.

---

## 📡 How GPS Location Is Obtained

The app uses the device’s **location services** to retrieve GPS coordinates (latitude and longitude). Once permission is granted:

1. The app requests location updates from the device.
2. The current latitude and longitude are received.
3. These coordinates are displayed on a map.
4. A marker is updated whenever the device changes location.

This approach ensures accurate and real-time tracking while keeping the implementation lightweight.

---

## 🗺 Map Integration

* A map is displayed using a map service (e.g., Google Maps SDK).
* The user’s location is marked with a visible marker.
* The camera automatically moves to follow the user’s position.

To avoid security risks, **API keys are not committed publicly** and are stored securely using local configuration files.

---

## 🖼 Screenshots

The following screenshots are included in the repository under the `screenshots/` folder:

* **permission_request.png** – Shows runtime location permission prompt
* **map_location.png** – Displays the map with the user’s current location marker
* **location_update.png** – Demonstrates marker movement when the device changes location

---

## 📂 Repository Structure

```
MobileDev-StudentName/
│
├── app/
│   └── source code
├── screenshots/
│   ├── permission_request.png
│   ├── map_location.png
│   └── location_update.png
├── README.md
```

---

## ⚠ Common Pitfalls Avoided

* Runtime permissions are properly requested and handled
* App does not crash if location permission is denied
* Only basic map features are used to keep the app simple
* API keys are not exposed in the public repository

---

## 🔍 Key Takeaway

Device sensors and features such as **GPS** allow mobile applications to interact with the physical world. By integrating location services and maps responsibly, developers can build **context-aware applications** while respecting user privacy and device limitations.
