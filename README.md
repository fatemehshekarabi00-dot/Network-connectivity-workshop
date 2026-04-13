# Network Connectivity Demo

A simple iOS demo project showing how devices can connect and communicate over a local network using Bonjour and Apple’s Network framework.

This project is designed for learning and workshop purposes.

---

##  Features

- Host / Join flow  
- Device discovery using Bonjour  
- TCP connection using Network framework  
- Send and receive simple text messages  
- Multiple devices can connect to the same session  

---

##  How It Works

This app demonstrates three main steps of network connectivity:

1. Discovery  
Devices find each other using Bonjour  

2. Connection  
A TCP connection is established using NWConnection  

3. Data Transfer  
Messages are sent and received between devices  

---

## 🛠 Requirements

- iOS 15+  
- Xcode 15+  
- Devices connected to the same Wi-Fi network  

---

##  Important Setup (Required)

To make device discovery work, you must enable Bonjour in your app:

1. Open your project settings  
2. Go to Info.plist  
3. Add:

Bonjour services  
_demo._tcp  

4. Also add:

Privacy - Local Network Usage Description  

With a value like:

This app uses the local network to discover nearby devices.  

Without this step, devices will NOT be able to discover each other.

---

##  How to Run

1. Run the app on two or more real devices  
2. Make sure all devices are on the same Wi-Fi network  

On one device:
- Tap Host  

On other devices:
- Tap Join  
- Select the host from the list  

Then:
- Send messages between devices  

---

##  Notes

- This is a minimal demo for learning purposes  
- No advanced error handling is included  
- Focus is on understanding the core connectivity flow  

---

##  Author

Fatima
