# 🌾 GramaSethu

### AI-Powered Rural Connectivity & Flood Safety Platform

GramaSethu is an Android application designed to improve rural connectivity and safety by helping communities monitor bridge conditions, report hazards, receive flood-related alerts, and access AI-assisted safety guidance.

The application combines **real-time community reporting, map-based bridge monitoring, Firebase-backed data, location services, and an AI safety assistant** into a single mobile platform.

---

## 🚨 Problem

Rural communities can face serious transportation and safety challenges during heavy rainfall and flooding.

Some common problems include:

- Bridges becoming unsafe or submerged during floods
- Limited access to timely road and bridge condition information
- Difficulty reporting damaged infrastructure
- Lack of centralized community safety information
- Uncertainty about safe routes during heavy rainfall
- Limited access to simple, location-aware safety guidance

GramaSethu was designed as a technology-driven approach to address these challenges.

---

## 💡 Solution

GramaSethu provides a centralized mobile platform where users can:

- View bridge conditions on an interactive map
- Identify safe, warning, and submerged bridges
- Submit community reports about local infrastructure
- Share flood and road safety information
- Receive alerts about reported hazards
- Use an AI assistant for flood and travel safety guidance
- Manage their profile and view submitted reports

The goal is to connect **community reporting + location data + real-time infrastructure information + AI assistance** in one application.

---

## ✨ Key Features

### 🗺️ Interactive Bridge Map

- Google Maps integration
- Bridge locations displayed on the map
- Visual bridge status indicators
- Safe, warning, and submerged bridge conditions
- Location-based map experience

### 🌉 Bridge Safety Monitoring

Users can view bridge conditions based on available data.

Bridge states include:

- 🟢 **OPEN** — bridge currently reported as open
- 🟡 **WARNING** — potentially unsafe conditions
- 🔴 **SUBMERGED** — bridge should be avoided

---

### 📢 Community Reporting

Users can submit reports about local infrastructure and safety conditions.

Reports can include:

- Location
- Local infrastructure information
- Report details
- Community-submitted safety information

This allows users to contribute local information that can help other people in the area.

---

### 🚨 Safety Alerts

The application provides an alert-oriented interface for community safety information.

Users can access information related to:

- Flood conditions
- Bridge hazards
- Road safety
- Community reports
- Unsafe travel conditions

---

### 🤖 AI Safety Assistant

GramaSethu includes an AI-powered assistant focused on rural flood and road safety.

The assistant can provide guidance about:

- Bridge safety
- Flood precautions
- Safe travel
- Alternative routes
- Heavy rainfall
- Monsoon preparation
- Emergency actions during flooding
- General rural road safety

The AI layer is implemented through a dedicated repository and HTTP API integration. The current source uses the **Groq API with Llama 3.3 70B Versatile**, while the API key is intentionally replaced with a placeholder in the public repository. 

---

### 👤 User Profile

Users can access their profile and manage application-related information.

The application also includes report history functionality for community submissions.

---

### 🔐 Authentication

The project includes an authentication-oriented application flow and Firebase integration.

Authentication and backend configuration are intentionally excluded from the public repository where credentials would otherwise be required.

---

### 🎨 Modern Android UI

The application is built using **Jetpack Compose** and includes:

- Material-based UI
- Animated screens
- Loading states
- Custom navigation
- Reusable UI components
- Splash screen
- Responsive layouts

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| **Kotlin** | Primary programming language |
| **Jetpack Compose** | Android UI development |
| **Firebase** | Backend/data services |
| **Google Maps** | Interactive maps and locations |
| **Groq API** | AI assistant |
| **Llama 3.3 70B Versatile** | AI model used by the assistant |
| **OkHttp** | HTTP networking |
| **Kotlin Coroutines** | Asynchronous operations |
| **Android Studio** | Development environment |
| **Git & GitHub** | Version control |

---

## 🏗️ Project Architecture

The application follows a simple separation between UI, data, and application logic.

```text
GramaSethu
│
├── app
│   │
│   └── src
│       │
│       ├── androidTest
│       │
│       ├── main
│       │   │
│       │   ├── java
│       │   │   └── com.example.gramasethu
│       │   │       │
│       │   │       ├── MainActivity.kt
│       │   │       │
│       │   │       ├── data
│       │   │       │   ├── AlertRepository.kt
│       │   │       │   ├── BridgeRepository.kt
│       │   │       │   ├── CustomReportRepository.kt
│       │   │       │   ├── GeminiRepository.kt
│       │   │       │   └── ReportRepository.kt
│       │   │       │
│       │   │       └── ui
│       │   │           ├── components
│       │   │           ├── navigation
│       │   │           ├── screens
│       │   │           └── theme
│       │   │
│       │   └── res
│       │
│       ├── test
│       └── androidTest
│
└── README.md
