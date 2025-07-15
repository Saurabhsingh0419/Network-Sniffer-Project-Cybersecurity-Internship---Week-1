
---

## 📄 `report.md`

```markdown
# 📑 Week 1 Cybersecurity Internship Report

## 🔐 Project Title:
**Network Sniffer and Log Analysis**

---

## 📌 Objective:
Build a Python script using **Scapy** to sniff live network packets and log them into an **SQLite3 database**. Verify the captured logs using SQLite CLI.

---

## 📦 Tools & Technologies:

- Python 3.13.2
- Scapy
- SQLite3 (v3.50.2 CLI)
- VS Code
- Windows 11

---

## 📈 Process:

1. Installed Scapy and SQLite3.
2. Created `sniffer.py` to capture packets, extract:
   - Timestamp
   - Source & Destination IP
   - Source & Destination Port
   - Length
   - TCP Flags
3. Stored each record into `packet_logs.db`.
4. Configured Windows Environment Variables for SQLite3.
5. Verified SQLite installation via CLI.
6. Queried the database to view captured logs.

---

## 📸 Screenshots:

- Sniffer output in terminal.
- SQLite3 version confirmation.
- Logs saved and viewed in SQLite3.

---

## 🎯 Outcome:

Successfully built and tested a functional packet sniffer that captures live traffic and logs essential details into a SQLite database, verified via CLI.

---

## 📚 Learnings:

- Live network traffic interception.
- Database management through Python.
- Environment variable management on Windows.
- Practical exposure to CLI-based SQLite.
