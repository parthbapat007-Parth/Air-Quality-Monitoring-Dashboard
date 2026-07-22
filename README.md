# Air Quality Monitoring Dashboard

A real-time web-based Air Quality Monitoring Dashboard that provides location-based environmental information using the **World Air Quality Index (WAQI) API**. The application automatically detects the user's current location, retrieves live air quality data, and presents it through a clean, responsive, and interactive dashboard.

This project was developed as a **Third Year B.Sc. Computer Science Group Project** to demonstrate the practical implementation of API integration, full-stack web development, and real-time environmental data visualization using Python Flask.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Technology Stack](#technology-stack)
- [Project Structure](#project-structure)
- [Project Preview](#project-preview)
- [Working Principle](#working-principle)

---

# Overview

Air pollution has become one of the most significant environmental challenges affecting human health and the environment. Although many online platforms provide air quality information, most require manual location input or display generalized data that may not accurately represent the user's surroundings.

The **Air Quality Monitoring Dashboard** solves this problem by automatically detecting the user's current location and displaying real-time environmental information through an intuitive web interface.

Using the **Browser Geolocation API**, the application captures the user's latitude and longitude and securely sends them to a **Flask backend**, which communicates with the **World Air Quality Index (WAQI) API**. The backend processes the API response and returns only the required information to the frontend for display.

The dashboard provides real-time information such as:

- Air Quality Index (AQI)
- PM2.5 Concentration
- PM10 Concentration
- Carbon Dioxide (CO₂)
- Temperature
- Humidity
- Weather Conditions
- Air Quality Graphs

This project demonstrates practical implementation of:

- REST API Integration
- Client-Server Architecture
- Browser Geolocation API
- JSON Data Processing
- Responsive Web Development
- Python Flask Backend

---

# Features

- Automatic location detection using Browser Geolocation API.
- Real-time Air Quality Index (AQI) monitoring.
- Live PM2.5 and PM10 concentration values.
- Carbon Dioxide (CO₂) monitoring.
- Temperature and humidity information.
- Current weather conditions.
- Dynamic graphical representation of environmental data.
- Responsive design for desktop and mobile devices.
- Flask-based backend for secure API communication.
- JSON data parsing and processing.
- Fast and lightweight application.
- Easy deployment and maintenance.
- Modular architecture for future scalability.

---

# Technology Stack

| Category | Technologies |
|----------|--------------|
| Frontend | HTML5, CSS3, JavaScript |
| Backend | Python, Flask |
| API | World Air Quality Index (WAQI), Browser Geolocation API |
| Libraries | Flask, Requests |
| Development Tools | Visual Studio Code, Git, GitHub |
| Browser Support | Google Chrome, Microsoft Edge, Mozilla Firefox |

---

# Project Structure

```text
Air-Quality-Monitoring-Dashboard/
│
├── Assets/
│   ├── HOME.png
│   ├── Location_Permission.png
│   ├── current_weather.png
│   └── Graph.png
│
├── Documents/
│   └── Tech_For_Air_Quality_Monitoring.pdf
│
├── static/
│   ├── css/
│   ├── js/
│   └── images/
│
├── templates/
│   └── index.html
│
├── app.py
├── requirements.txt
├── README.md
└── .gitignore
```

The project follows a client-server architecture where the frontend communicates with a Flask backend, which retrieves real-time environmental data from the WAQI API and returns the processed information to the dashboard.

---

# Project Preview

## Home Page

![Home Page](Assets/HOME.png)

The home page introduces the dashboard and provides users with a clean interface to begin monitoring air quality based on their current location.

---

## Location Permission

![Location Permission](Assets/Location_Permission.png)

The application requests permission to access the user's location using the Browser Geolocation API. Once permission is granted, the geographical coordinates are securely sent to the Flask backend.

---

## Current Weather & Air Quality Dashboard

![Dashboard](Assets/current_weather.png)

The dashboard displays real-time environmental information including:

- Air Quality Index (AQI)
- PM2.5
- PM10
- Carbon Dioxide (CO₂)
- Temperature
- Humidity
- Weather Conditions

All information is retrieved dynamically through the WAQI API.

---

## Air Quality Graph

![Air Quality Graph](Assets/Graph.png)

The graphical visualization provides an easy-to-understand representation of air quality data, allowing users to compare environmental parameters more effectively.

---

# Working Principle

The Air Quality Monitoring Dashboard follows a simple client-server workflow.

1. The user opens the web application.

2. The browser requests permission to access the user's current location.

3. The Browser Geolocation API retrieves the latitude and longitude.

4. The coordinates are sent securely to the Flask backend.

5. Flask creates a request to the World Air Quality Index (WAQI) API.

6. The WAQI API returns environmental information in JSON format.

7. Flask extracts the required parameters.

8. The processed data is sent back to the frontend.

9. The dashboard updates automatically and displays:

   - Air Quality Index (AQI)
   - PM2.5
   - PM10
   - Carbon Dioxide (CO₂)
   - Temperature
   - Humidity
   - Weather Information
   - Air Quality Graphs

---

> Continue to **Part 2** for the complete system architecture, API workflow, installation guide, advantages, limitations, and documentation.
