##🌱 Smart Irrigation System

A Smart Irrigation System using **Arduino**, **Flask**, and **React** to automate garden or field watering based on real-time soil moisture sensor data.

## 🚀 Features

- Live soil moisture monitoring
- Automated irrigation control
- Historical moisture data chart
- Manual irrigation override
- Real-time communication between Arduino and server
- Modern React dashboard for control and insights

---

## 🛠️ Tech Stack

- **Frontend:** React.js, Chart.js, Axios
- **Backend:** Flask (Python), pySerial, Flask-CORS
- **Hardware:** Arduino UNO / ESP32, Soil Moisture Sensor, Relay Module, Pump

---

## 🔌 Hardware Requirements

- Arduino UNO or ESP32
- Soil Moisture Sensor (e.g., YL-69)
- Relay Module
- Water Pump
- Jumper Wires + Breadboard
- USB cable for Arduino connection

---

📁 **Project Structure**

smart-irrigation/
│
├──    backend/
│     ├── app.py
│     ├── serial_reader.py
│     ├── scheduler.py
│     ├── .env
│     └── requirements.txt
│
      ├── frontend/
│     ├── public/
│     └── src/
│     ├── App.js
│     ├── components/
│     └── services/
│
└── README.md

---

## ⚙️ Setup Instructions

### 🔧 Backend (Flask)

1. Navigate to the backend folder:
   cd backend
**Create and activate a virtual environment:**
python -m venv venv
venv/bin/activate
# On Windows: venv\Scripts\activate

**Install dependencies:**
pip install -r requirements.txt
**Run the Flask server:**
python app.py

**🌐 Frontend (React)**
Navigate to the frontend folder:

cd frontend

**Install frontend dependencies:**

npm install

**Start the development server:**

npm start

🔄 **Arduino SetupArduino Setup (with PlatformIO)**
Open the firmware/ folder in VS Code with PlatformIO and install the PlatformIO extension on VS code.


📊 **API Endpoints (Flask)** 

Endpoint	Method	Description

/moisture	GET	Returns current soil moisture
/irrigate/on	POST	Turns irrigation on
/irrigate/off	POST	Turns irrigation off

