# 📱 VQueue - Offline Queue Management via Bluetooth LE

> [cite_start]**Showcase Repository**: VQueue is a native Android application developed as a team project for the **"Application Development for Mobile Devices" (TAMa)** course at **Brno University of Technology (FIT VUT)** during an **Erasmus+ mobility**.

---

## 📋 Overview
[cite_start]VQueue provides a convenient offline alternative to physical lines, allowing users to queue within a 100-meter range using **Bluetooth Low Energy (BLE)**[cite: 1]. [cite_start]The system requires **no internet, no sign-up, and no account creation**[cite: 1, 6].

---

## 🚀 Key Features
* [cite_start]**Completely Offline**: Works anywhere without Wi-Fi or cellular data using a custom P2P BLE protocol[cite: 1, 5].
* [cite_start]**Unlimited Client Support**: Solves the standard BLE limit (~7 connections) through a **Hybrid Architecture** combining transactional GATT connections with passive Advertising API broadcasting.
* [cite_start]**Real-Time Updates**: Customers track their position and progress bar in real-time[cite: 5].
* [cite_start]**Manual Management**: Queue managers can manually add people (without phones or iPhones) and pause the queue at any time[cite: 5].
* [cite_start]**Persistent States**: Integrated **Room Database** ensures queue info and turns are not wiped if the process is killed[cite: 3].

---

## 🛠 Tech Stack
* [cite_start]**Language**: **Java** & **XML** (Native Android SDK).
* [cite_start]**Platform**: Targets Android 15 with compatibility back to Android 5.0 (SDK 21).
* **Libraries (Jetpack)**: 
    * [cite_start]**Room DB**: For local data persistence[cite: 3].
    * [cite_start]**ViewModel**: To survive screen rotations and separate UI logic[cite: 3].
    * [cite_start]**Navigation Component**: For seamless Fragment transitions[cite: 3].
* [cite_start]**UI/UX**: **Material Design 2.0** with automatic light/dark theming based on user preferences[cite: 1, 5].

---

## 🏗 Technical Challenge & Discovery
[cite_start]The biggest challenge was bypassing the physical connection limits of BLE[cite: 5]. 
* [cite_start]**The Solution**: A custom data exchange protocol using **byte packing** to fit app identification, queue info, and status into tiny 19-byte BLE packets[cite: 6].
* [cite_start]**Architecture**: A single-activity, fragment-based **MVC approach**[cite: 6].

---

## 🌍 Context & Team
* [cite_start]**Institution**: Faculty of Information Technology, Brno University of Technology.
* [cite_start]**Team**: Eyobed A. Nuri (Lead/BLE), **Lucas Labhini (UI/Bugs/Docs)**, Adam Selmane (BLE/RSSI), Krystof Michalek (Setup/Bugs), Kaung San (UI/Tests)[cite: 1, 4].

---

## 📋 About this Showcase
This repository is a demonstration of native mobile development and low-level hardware access.
* **Code Status**: Private collaborative academic project.
* [cite_start]**App Size**: Ultra-lightweight (1.5 MB)[cite: 6].
* **Assets**: Includes technical documentation and the compiled APK.

---
*Developed during an Erasmus+ mobility at VUT Brno.*
