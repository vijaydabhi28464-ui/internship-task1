# internship-task1
Local Network Port Scanning using Nmap
# Task 1 – Local Network Port Scanning

# Objective
To scan the local network for open ports and identify exposed services using Nmap.



## 🛠 Tools Used
- Nmap
- kali linux

---

## Methodology

### Step 1: Identify Local IP Range
Used `ipconfig` to determine:
IPv4: 192.168.195.131
Subnet: 255.255.255.0
Range: 192.168.1.0/24

### Step 2: Perform TCP SYN Scan
Command used:
nmap -sS 192.168.195.131/24

### Step 3: Save Scan Results
nmap -sS 192.168.195.131/24 -oN scan_results.txt

---

## 📊 Findings

| IP Address | Open Ports | Services |
|------------|------------|----------|
| 192.168.195.131| 22 | SSH |

---

## ⚠️ Identified Risks

- SSH (22) could be targeted by brute force attacks.
- Open ports increase attack surface.

---

## 🔐 Security Recommendations

- Disable unused services.
- Use strong authentication..
- Restrict SSH access.

---

## 📁 Repository Structure

cybersecurity-task1-port-scan/
│
├── scan_results.txt
├── screenshots/
│   ├── nmap_output.png
└── README.md

---

## 🧠 Key Concepts Learned

- Port scanning
- TCP SYN (Stealth) Scan
- Network reconnaissance
- Service exposure analysis
- Basic security risk assessment

---

## ⚖️ Ethical Consideration

Scanning was performed only on my own local network for educational purposes.
