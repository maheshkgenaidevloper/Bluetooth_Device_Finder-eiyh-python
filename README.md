# Bluetooth_Device_Finder-eiyh-python
# 📡 Bluetooth Radar — Device Finder Using Python

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white">
  <img src="https://img.shields.io/badge/Bluetooth-BLE-0082FC?style=for-the-badge&logo=bluetooth&logoColor=white">
</p>

<p align="center">
  <b>Discover nearby BLE devices through an interactive Python dashboard.</b>
</p>

## ✨ Features

- 🔍 Scan nearby Bluetooth Low Energy advertisements
- 📱 Display device names and addresses when available
- 📶 View RSSI signal strength
- 📊 Categorize signal strength
- 🔎 Search discovered devices
- 📥 Export results to CSV
- 🖥️ Interactive Streamlit dashboard

## 🛠️ Tech Stack

- Python
- Bleak
- Streamlit
- Pandas

## 📂 Project Structure

```text
Bluetooth-Device-Finder/
├── app.py
├── requirements.txt
├── README.md
└── .gitignore
```

## 🚀 Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/Bluetooth-Device-Finder.git
cd Bluetooth-Device-Finder
```

Replace `YOUR_USERNAME` with your GitHub username.

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Windows:

```powershell
.\.venv\Scripts\Activate.ps1
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Start the application

```bash
python -m streamlit run app.py
```

Open `http://localhost:8501` in your browser if it does not open automatically.

## 📊 How It Works

1. The user selects a scan duration.
2. Bleak scans for nearby BLE advertisements.
3. The app extracts available device names, addresses,
   signal strength, and service UUIDs.
4. Streamlit displays the results in a table.
5. The user can search and download the results as CSV.

## ⚠️ Important Limitations

- This project scans BLE advertisements, not every classic Bluetooth device.
- Devices that are not advertising may not appear.
- RSSI is not a precise distance measurement.
- Device addresses may be unavailable or randomized.
- Bluetooth hardware, drivers, and operating-system permissions affect scanning.

## 🔐 Responsible Use

Use the scanner only for legitimate, authorized discovery.
Do not publish scan exports containing sensitive device information.

## 🔮 Future Improvements

- Signal-strength history charts
- Scan history
- Service UUID filters
- Improved dashboard visualizations
- Automated tests

## 📜 License

Add an appropriate open-source license before permitting reuse.

---

<p align="center">
  ⭐ If you find this project useful, give the repository a star!
</p>
