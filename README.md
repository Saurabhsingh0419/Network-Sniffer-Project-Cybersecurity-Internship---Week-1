# 🕵️‍♂️ Network Sniffer with Anomaly Detection

This project is a Python-based **Network Packet Sniffer** that captures, logs, and detects suspicious network activity (like port scans or floods).  
Packets are stored in an **SQLite database**, and alerts are raised when thresholds are exceeded.

---

## **Features**
✔️ Capture live network packets using `scapy`  
✔️ Store packets with details (src/dst IP, ports, flags, length, timestamp) in SQLite  
✔️ Detect anomalies (Port Scan / Flooding) using thresholds  
✔️ Store alerts in DB and show in terminal  

---

## **How to Run**

1. Clone the repository:
   ```bash
   git clone <your-repo-url>
   cd network-sniffer-project

