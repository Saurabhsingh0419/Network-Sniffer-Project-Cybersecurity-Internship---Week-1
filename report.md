# 📝 Cybersecurity Internship Final Project Report

## **Project Title:**  
**Network Sniffer with Anomaly Detection**

---

## **Objective:**  
To develop a Python-based network packet sniffer that captures live traffic, logs essential details into an SQLite database, and detects anomalies (like port scans or flooding) in real-time.

---

## **Tools & Technologies Used:**  
- **Python 3.13**
- **Scapy** (for packet sniffing)
- **SQLite3** (for local database)
- **VS Code** (development environment)
- **Windows 11** (operating system)

---

## **Project Description:**  

### **Week 1:**  
- Implemented basic packet sniffer using **Scapy**.  
- Captured and logged details:
  - Timestamp  
  - Source IP & Destination IP  
  - Source Port & Destination Port  
  - Packet Length  
  - TCP Flags  
- Stored captured data into a local **SQLite3 database** (`packet_logs.db`).  
- Verified the database using **SQLite CLI**.  

### **Week 2:**  
- Added **Anomaly Detection** logic:
  - Tracked number of packets from each source IP within a **10-second window**.  
  - Triggered alert if packet count exceeded a defined threshold (**10 packets in 10 seconds**).  
- Created a new **Alerts Table** in the database to log all anomalies.  
- Displayed real-time alerts in terminal when suspicious activity was detected.  

---

## **Database Design:**  

**`packets` table:**  
| Column      | Type    | Description                  |
|-------------|---------|------------------------------|
| timestamp   | TEXT    | Packet capture time          |
| src_ip      | TEXT    | Source IP address            |
| dst_ip      | TEXT    | Destination IP address       |
| sport       | INTEGER | Source port                  |
| dport       | INTEGER | Destination port             |
| length      | INTEGER | Packet size in bytes         |
| flags       | TEXT    | TCP flags                    |

**`alerts` table:**  
| Column      | Type    | Description                  |
|-------------|---------|------------------------------|
| timestamp   | TEXT    | Time of alert                |
| src_ip      | TEXT    | Source IP that triggered alert|
| alert       | TEXT    | Alert message                |

---

## **Screenshots:**  
1. Sniffer running and capturing packets  
2. Database records (packets table)  
3. Alerts triggered during anomaly detection  
4. Verified database with SQLite CLI  

*(Screenshots are included in the `/screenshots/` folder)*  

---

## **Learnings:**  
- Practical experience with **packet-level network monitoring**.  
- Worked with **Scapy** for capturing and analyzing traffic.  
- Integrated **SQLite** with Python for persistent storage.  
- Designed and implemented a basic **anomaly detection** system.  
- Understood challenges like **database corruption handling** and **environment variable setup**.  

---

## **Future Scope:**  
- Add a **web dashboard** for real-time monitoring.  
- Export captured logs in **CSV/JSON** for further analysis.  
- Extend anomaly detection using **ML-based models** for advanced threat detection.  

---

## **Conclusion:**  
This project helped me understand how packet sniffers work at the network layer, how to analyze traffic, and how to design simple detection mechanisms to enhance network security.  

