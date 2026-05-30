# Eco-Grid RESONEX Dashboard

## Smart Infrastructure Monitoring & Sustainable Energy Management Platform

Eco-Grid RESONEX is a real-time monitoring dashboard designed for intelligent infrastructure surveillance, structural health analysis, public safety monitoring, and renewable energy tracking. The system integrates ESP32-based sensor networks with a modern React dashboard to provide live insights into critical urban infrastructure.

---

# Quick Setup (No Hardware Required)

Follow these steps to run the dashboard immediately using simulated data.

## Step 1 — Install Node.js

Download and install the latest **LTS (Long-Term Support)** version of Node.js:

https://nodejs.org

---

## Step 2 — Create a Vite React Project

Open a terminal and run:

```bash
npm create vite@latest eco-grid-resonex-dashboard -- --template react
cd eco-grid-resonex-dashboard
```

---

## Step 3 — Replace Source Files

Replace the contents of the `src/` folder with the provided project files:

```text
src/
├── index.css
├── main.jsx
├── App.jsx
├── data/
│   └── mockData.js
├── components/
│   ├── TopBar.jsx
│   ├── MetricCards.jsx
│   ├── VibrationChart.jsx
│   ├── SafetyPanel.jsx
│   ├── EnergyPanel.jsx
│   └── AlertsFeed.jsx
```

Also replace:

```text
package.json
vite.config.js
```

with the versions provided for the project.

---

## Step 4 — Install Dependencies

Install required packages:

```bash
npm install
npm install recharts lucide-react
```

---

## Step 5 — Start the Dashboard

Launch the development server:

```bash
npm run dev
```

Open your browser and navigate to:

```text
http://localhost:5173
```

The dashboard will load using simulated data, allowing testing without hardware.

---

# Hardware Integration (When ESP32 Arrives)

## Upload Firmware

Open:

```text
esp32_firmware.ino
```

in Arduino IDE.

Select:

```text
Tools → Board → ESP32S3 Dev Module
```

Upload the firmware to your ESP32-S3 board.

---

## Connect to Dashboard

### Recommended Browser

Use:

* Google Chrome
* Microsoft Edge

⚠️ Firefox does not support WebSerial.

---

### Connect Device

1. Open the Eco-Grid RESONEX Dashboard.
2. Click **Connect ESP32**.
3. Select the ESP32 COM Port.
4. Authorize WebSerial access.

Live sensor data will begin streaming automatically.

---

# Dashboard Features

## Real-Time Structural Monitoring

Live vibration analysis for:

* Flyover Structures
* Metro Pillars
* Streetlight Poles

Features include:

* Real-time sensor charts
* Historical trend visualization
* Continuous health assessment

---

## Structural Health Score

AI-powered infrastructure assessment displayed as:

```text
0% – 100%
```

Health levels:

| Score Range | Status   |
| ----------- | -------- |
| 80–100      | Healthy  |
| 60–79       | Warning  |
| Below 60    | Critical |

---

## Smart Guardian Safety Panel

Integrated public safety monitoring using:

* PIR Motion Detection
* Acoustic Event Detection
* Emergency SOS Alerts

Capabilities include:

* Intrusion monitoring
* Emergency event reporting
* Public safety notifications

---

## Sustainable Energy Monitoring

Live renewable energy tracking:

### Solar Generation

Monitor solar harvesting performance.

### Wind Generation

Track wind turbine energy output.

### Battery Storage

View battery charge and utilization levels.

Interactive energy bars provide real-time visualization.

---

## Live Event & Alert Feed

Continuous event logging with timestamps.

Examples:

* Structural vibration anomalies
* Motion detection events
* Emergency SOS activations
* Power system warnings
* Energy generation updates

Critical events are highlighted instantly.

---

# System Architecture

```text
ESP32 Sensors
        ↓
WebSerial Communication
        ↓
React + Vite Dashboard
        ↓
Real-Time Analytics Engine
        ↓
Structural Health Assessment
        ↓
Safety Monitoring
        ↓
Energy Management Visualization
```

---

# Technology Stack

| Layer                | Technology    |
| -------------------- | ------------- |
| Frontend             | React.js      |
| Build Tool           | Vite          |
| Charts               | Recharts      |
| Icons                | Lucide React  |
| Communication        | WebSerial API |
| Edge Hardware        | ESP32-S3      |
| Programming Language | JavaScript    |
| Styling              | CSS3          |
| Runtime              | Node.js       |

---

# Key Advantages

✅ No cloud dependency required

✅ Real-time monitoring

✅ Modern responsive UI

✅ Direct ESP32 communication

✅ Renewable energy visualization

✅ Public safety integration

✅ Structural health analytics

✅ Scalable smart-city deployment

---

# Future Scope

### Infrastructure Intelligence

* AI-based anomaly prediction
* Predictive maintenance scheduling
* Automated fault classification

### Smart City Expansion

* Traffic monitoring integration
* Smart streetlight management
* Environmental sensing modules

### Renewable Energy Optimization

* Solar forecasting
* Battery optimization algorithms
* Micro-grid management

### Emergency Response Systems

* Disaster detection
* Emergency notification network
* Citizen safety platform

---

# Conclusion

Eco-Grid RESONEX combines infrastructure monitoring, public safety intelligence, and renewable energy management into a unified dashboard platform. By leveraging ESP32 edge devices, WebSerial communication, and modern React-based visualization, the system provides an affordable and scalable solution for future smart-city deployments.

---

## License

Developed under the Eco-Grid RESONEX Initiative.

© 2026. All Rights Reserved.
