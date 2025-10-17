# Phoenix College NASA ASCEND Program

A comprehensive high-altitude ballooning project funded by the Arizona Space Grant Consortium, featuring advanced Arduino data collection systems and a modern web platform.

## 🚀 Project Overview

The NASA ASCEND program provides undergraduate STEM students with hands-on experience in real-world NASA-related science and engineering projects. Our team has developed a sophisticated data collection system for high-altitude balloon missions, complete with sensor integration, GPS tracking, and data visualization.

## 🌐 Live Website

**Visit our live website:** [https://prestonfurulie.github.io/NASA/](https://prestonfurulie.github.io/NASA/)

## 📁 Project Structure

```
NASA/
├── site/                          # Website source code
│   ├── src/
│   │   ├── pages/                # Website pages
│   │   │   ├── index.astro       # Main homepage
│   │   │   ├── dashboard.astro   # Member dashboard
│   │   │   ├── arduino-code.astro # Arduino code showcase
│   │   │   ├── mission-data.astro # Mission data visualization
│   │   │   └── documentation.astro # Complete documentation
│   │   └── arduino/              # Arduino source code
│   │       ├── HailMaryV1b.ino   # Original working version
│   │       ├── HailMaryV1c_GPS.ino # GPS-integrated version
│   │       └── HailMaryV1c_NoGPS.ino # Clean version without GPS
│   └── dist/                     # Built website (auto-generated)
└── README.md                     # This file
```

## 🔧 Arduino Data Collection System

### Hardware Components
- **Arduino Mega 2560** - Main microcontroller
- **Adafruit BMP390** - Pressure, temperature, altitude sensor (SPI)
- **Adafruit BNO055** - 9-axis IMU (gyroscope, accelerometer, magnetometer) via I2C
- **SparkFun AS7331** - UV sensors (4 units) via I2C
- **SD Card Module** - Data logging (SPI)
- **GPS Module** (optional) - NEO-6M for UTC timestamps

### Code Versions

#### HailMaryV1b.ino
- **Original working version** - Safe backup
- All sensors: BMP390, BNO055, AS7331 (x4), SD card
- Uses millis() timestamps
- Robust error handling and data validation

#### HailMaryV1c_GPS.ino
- **GPS-integrated version** - For accurate UTC timestamps
- All sensors from V1b PLUS GPS module
- UTC timestamps for time-series analysis
- GPS coordinates for trajectory mapping
- Graceful fallback if GPS unavailable

#### HailMaryV1c_NoGPS.ino
- **Clean version without GPS** - Simplified for basic missions
- All sensors from V1b (no GPS)
- Enhanced documentation
- Optimized for high-altitude balloon missions

## 🌐 Website Features

### Public Website
- **Responsive Design** - Works on all devices using Bootstrap 5
- **Modern UI** - Space-themed design with smooth animations
- **Project Showcase** - Display of Arduino data collection system
- **Mission Data** - Embedded videos and presentations
- **Team Information** - Program overview and team details
- **Contact System** - Easy application and contact forms

### Member Dashboard
- **Secure Login** - Authentication system for team members
- **Project Management** - Track active projects and progress
- **Data Visualization** - Interactive charts and mission data
- **Resource Library** - Access to code, documentation, and files
- **Team Collaboration** - Member profiles and communication tools
- **Real-time Updates** - Live data and status monitoring

## 🔐 Demo Access

### Member Login Credentials
- **Project Lead**: `pre2167119@maricopa.edu` / `ascend2024`
- **Admin**: `admin@phoenixcollege.edu` / `admin123`
- **Student**: `student@phoenixcollege.edu` / `student123`

## 📊 Mission Data

Our system collects comprehensive data from high-altitude balloon missions:
- **Environmental Data**: Pressure, temperature, altitude profiles
- **Motion Data**: Gyroscope and accelerometer readings
- **UV Radiation**: Multi-spectral UV measurements
- **GPS Tracking**: Real-time position and trajectory data
- **Timestamps**: Precise UTC timing for data correlation

## 🛠️ Technology Stack

### Frontend
- **Astro** - Modern static site generator
- **Bootstrap 5** - Responsive UI framework
- **Chart.js** - Data visualization
- **Bootstrap Icons** - Icon library

### Backend
- **GitHub Pages** - Static hosting
- **Local Storage** - Client-side authentication
- **Chart.js** - Real-time data visualization

### Hardware
- **Arduino Mega 2560** - Microcontroller
- **Multiple Sensors** - Environmental and motion sensing
- **SD Card** - Data storage
- **GPS Module** - Position tracking

## 🚀 Getting Started

### For Website Development
1. Clone the repository
2. Install dependencies: `npm install`
3. Start development server: `npm run dev`
4. Build for production: `npm run build`

### For Arduino Development
1. Download Arduino IDE
2. Install required libraries (see documentation)
3. Upload appropriate .ino file to Arduino Mega
4. Connect hardware according to wiring diagrams

## 📚 Documentation

Complete documentation is available on the website:
- **Hardware Setup** - Detailed wiring diagrams and component guides
- **Software Guide** - Code installation and configuration
- **Data Analysis** - Tools and techniques for mission data
- **Mission Operations** - Pre-launch, launch, and recovery procedures

## 👥 Team Members

- **Preston Furulie** - Project Lead, Arduino Development, Hardware Integration
- **Angela Trainor** - Software Engineer, Data Analysis, Visualization
- **Marquis Muza** - Hardware Engineer, Sensor Integration, PCB Design
- **Ethan Pierson** - Data Scientist, Mission Analysis, Statistics

## 📈 Mission Statistics

- **12** Missions Completed
- **28,500m** Peak Altitude Achieved
- **-52°C** Minimum Temperature Recorded
- **4.2 hours** Average Flight Duration
- **45,678** Data Points Collected

## 🔗 Links

- **Live Website**: [https://prestonfurulie.github.io/NASA/](https://prestonfurulie.github.io/NASA/)
- **Arduino Repository**: [https://github.com/PrestonFurulie/arduino](https://github.com/PrestonFurulie/arduino)
- **Phoenix College**: [https://www.phoenixcollege.edu/](https://www.phoenixcollege.edu/)
- **Arizona Space Grant**: [https://spacegrant.arizona.edu/](https://spacegrant.arizona.edu/)

## 📄 License

Phoenix College NASA ASCEND Project - Educational Use

## 🤝 Contributing

This project is part of the Phoenix College NASA ASCEND program. For questions or collaboration opportunities, please contact the team at ascend@phoenixcollege.edu.

---

**Built with ❤️ by the Phoenix College NASA ASCEND Team**