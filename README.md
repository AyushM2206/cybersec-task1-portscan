# Cyber Security Internship – Task 1: Network Port Scanning

## 👨‍💻 Performed By:
Ayush

## 🧾 Objective:
To perform a TCP SYN scan using Nmap and identify open ports and services on devices in the local network.

---

## 🧰 Tools Used:
- Nmap (Version 7.97)
- Windows 10 Command Prompt

---

## 🌐 IP Range Scanned:
`172.20.10.0/28`

---

## 📊 Scan Results:

### ▶ 172.20.10.1
- Open Ports: 21 (FTP), 53 (DNS), 49152 (Unknown), 62078 (iPhone-sync)
- Notes: Port 21 (FTP) is insecure if anonymous login is enabled. iPhone-sync may indicate a connected Apple device.

### ▶ 172.20.10.2
- Open Ports: 135 (MSRPC), 139 (NetBIOS-SSN), 445 (SMB), 3306 (MySQL)
- Notes: File sharing ports 139 & 445 are vulnerable if exposed externally. MySQL port should be firewalled.

---

## 🔐 Security Insights:
- **FTP** and **SMB** ports can be exploited if not properly secured.
- Services like **MySQL** must not be exposed to public networks.
- Unnecessary services should be disabled or firewalled.

---

## 📁 Files Included:
- `scan_results.txt` – Raw output from Nmap TCP SYN scan

---

## 📌 Conclusion:
This task helped understand how network reconnaissance works using Nmap. It gave insight into what services are running on devices in a network and how open ports can be a security concern.

