# Packet Analysis Tool

## 📌 Overview
This project implements a simple **Packet Analysis Tool** that captures live network traffic, analyzes it for potential security threats, and generates a report of the findings.

## 🎯 Objective
- Capture live packets using tools like **Wireshark**, **tcpdump**, or **Scapy**.
- Analyze captured packets for suspicious activity such as malicious IPs, unusual traffic patterns, or protocol anomalies.
- Generate a detailed report with findings and screenshots.

## 🛠 Tools & Technologies
- **Wireshark** – Packet capture and analysis
- **tcpdump** – Command-line packet analyzer (optional)
- **Scapy** – Python-based packet analysis (optional)
- **Operating System:** Windows/Linux

## 📂 Project Structure
```
Packet-Analysis-Tool/
│── Packet_Analysis_Tool_Report.docx   # Detailed project report
│── README.md                          # Project documentation (this file)
│── /screenshots                       # Wireshark screenshots (to be added)
```
(*Add screenshots in the `/screenshots` folder before pushing to GitHub*)

## 🚀 Steps to Run the Project
1. Install [Wireshark](https://www.wireshark.org/download.html) on your system.
2. Run Wireshark as **Administrator/Root** to allow packet capture.
3. Select your active network interface (Wi-Fi/Ethernet).
4. Start capturing packets and perform normal browsing activity.
5. Stop capture after a few minutes and save the `.pcapng` file.
6. Apply filters in Wireshark to analyze packets:
   - `http` → Web traffic
   - `dns` → DNS lookups
   - `tcp.port==443` → HTTPS traffic
   - `ip.addr==<IP>` → Filter by specific IP
7. Document your findings and update the project report.

## 📊 Example Findings
- Normal browsing traffic (Google, YouTube).
- DNS queries to `8.8.8.8` (Google DNS).
- No major threats detected in test capture.

## 📝 Report
The full project report is available in **Packet_Analysis_Tool_Report.docx**. 

## 🔗 References
- [Wireshark Documentation](https://www.wireshark.org/docs/)
- [Nmap Documentation](https://nmap.org/book/)
- [Scapy Documentation](https://scapy.readthedocs.io)
