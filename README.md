# 🛡️ Network Sniffer Project | Cybersecurity Internship - Week 1

A lightweight Python-based network sniffer built using **Scapy** that captures TCP/IP packets from the local network interface, extracts essential information, and logs it to an **SQLite3 database**.

---

## 📌 Objective

- Capture live network traffic.
- Extract:
  - Timestamp
  - Source IP
  - Destination IP
  - Source Port
  - Destination Port
  - Packet Length
  - TCP Flags
- Store the captured packet details in a local SQLite database.
- Verify data using SQLite CLI.

---

## 📦 Requirements

- Python 3.13+
- Scapy
- SQLite3 (CLI and Python module)

### Install Dependencies

```bash
pip install scapy
