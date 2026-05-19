# Battery Digital Twin

A Unity-based Digital Twin of a Lithium-Ion Battery with real-time sensor integration, Firebase cloud connectivity, machine learning-based SOC and SOH prediction, interactive gauges, real-time graphs, and 3D visualization.

---

## Project Overview

This project creates a virtual representation (Digital Twin) of a lithium-ion battery. Real-time data from physical sensors is transmitted to Firebase Realtime Database, where machine learning models predict:

* **State of Charge (SOC)**
* **State of Health (SOH)**

Unity retrieves both the sensor data and prediction results and displays them in a fully interactive 3D dashboard.

---

## System Architecture

1. Physical battery sensors connected to an ESP32 measure:

   * Voltage
   * Current
   * Temperature

2. Sensor data is uploaded to Firebase Realtime Database.

3. Machine learning models process the data and predict:

   * SOC
   * SOH

4. Predicted values are written back to Firebase.

5. Unity reads all real-time values from Firebase and updates:

   * Dashboard parameters
   * Battery status
   * Performance gauges
   * Real-time graphs
   * 3D cylindrical indicators
   * Floating information panels

---

## Features

* Real-time Firebase integration
* Machine learning SOC and SOH prediction
* Interactive Unity dashboard
* Dynamic semicircular gauges
* Real-time voltage, current, and temperature graph
* 3D battery visualization
* Battery status detection (Charging / Discharging / Idle)
* System log panel
* Floating parameter display
* SOC, SOH, and temperature cylinder indicators

---

## Technologies Used

* Unity 6
* C#
* Firebase Realtime Database
* ESP32
* Python
* Scikit-learn
* Random Forest Regression
* Google Colab / Jupyter Notebook

---

## Project Structure

* `Assets/Scripts/BatteryVisualizer.cs` – Updates dashboard, gauges, graph, and 3D objects
* `Assets/Scripts/FirebaseManager.cs` – Connects Unity to Firebase
* `Assets/Scripts/BatteryData.cs` – Data model for battery parameters
* `Assets/Scenes/SampleScene.unity` – Main digital twin scene

---

## Real-Time Parameters

* Cell ID
* Voltage (V)
* Current (A)
* Temperature (°C)
* SOC (%)
* SOH (%)
* Power (W)
* Battery Status

---

## Dashboard Components

* Main monitor panel
* Cell parameter panel
* Real-time graph
* Performance gauges
* Floating cell panel
* System log panel
* 3D SOC/SOH/Temperature cylinders

---

## Team Contribution

This project was developed as part of a collaborative academic project focused on battery monitoring, machine learning prediction, and digital twin technology.

---

## Future Scope

* Predictive maintenance and fault detection
* Battery Remaining Useful Life (RUL) estimation
* Multi-cell battery pack monitoring
* Web and mobile dashboard integration

---

## Author

Ayush Kumar and Team

---
