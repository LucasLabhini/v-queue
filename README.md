# 📱 VQueue - Offline Queue Management via BLE

> **Showcase Repository**: VQueue is a native Android application developed as a team project for the **"Application Development for Mobile Devices" (TAMa)** course at **FIT VUT Brno** during an **Erasmus+ mobility**. It provides a professional offline alternative to physical lines using a custom **Bluetooth Low Energy (BLE)** protocol to manage queues within a 100-meter range.

---

## 📋 Project Overview
VQueue is designed for environments without internet access (festivals, local shops, or rural centers). It allows users to join virtual lines, track their turn, and receive notifications—all without Wi-Fi, cellular data, or account creation.

---

## 🚀 Key Features
* **Hybrid BLE Architecture**: Bypasses the standard 7-connection limit of BLE by using brief **GATT connections** for the initial join, followed by **passive Advertising API broadcasting** for real-time status updates.
* **Custom P2P Protocol**: Features a high-efficiency data exchange protocol using **byte packing** to fit the application ID and queue status into 19-byte BLE packets.
* **Specialized Modes**:
    * **Queue Manager**: Create a queue, call the next person, or manually add users who do not have a smartphone.
    * **Customer Display**: Scans the area for active queues and displays real-time progress via a dedicated UI.
* **Persistence**: Integrated **Room Database** to ensure queue data is saved locally and survives if the app process is interrupted.

---

## 🛠 Tech Stack
* **Language**: **Java** and **XML** (Native Android SDK).
* **Tools**: Android Studio, targeting Android 15 (compatible down to Android 5.0).
* **Jetpack Libraries**: 
    * **Room DB**: Local state storage.
    * **ViewModel**: UI/Logic separation and rotation handling.
    * **Navigation Component**: Fragment-based single-activity architecture.
* **UI/UX**: **Material Design 2.0** with automated light/dark theme support.

---

## 🌍 Team & Context
This project was a collaborative effort at the Faculty of Information Technology, Brno University of Technology.
* **Team**: Eyobed A. Nuri (Lead/Logic), **Lucas Labhini (UI/Bugs/Docs)**, Adam Selmane (BLE Logic), Krystof Michalek (Setup), Kaung San (Tests).
* **My Contribution**: Developed the core concept, improved UI components, and fixed critical fragment navigation and instance bugs.

---

## 📦 Deliverables
* **[app-release.apk](./app-release.apk)**: Compiled Android package available for testing.
* **[Vqueue_presentation.pptx](./Vqueue_presentation.pptx)**: Project feature and design overview.

---

*Developed at FIT VUT Brno — 2025.*
