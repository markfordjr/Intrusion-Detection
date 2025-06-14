# Intrusion Detection System (IDS)

**📡 Network Traffic Analysis with Wireshark & SysInternals**

**Author:** Mark Ford Jr.

---

## 🔍 Overview

This project demonstrates how to build and test a lightweight Intrusion Detection System using **Wireshark** and **Microsoft SysInternals**. The goal was to detect suspicious activity within a simulated network environment by analyzing traffic, identifying anomalies, and reporting findings.

---

## 🎯 Objectives

* Capture and analyze real network traffic (200+ packets)
* Detect anomalies such as unusual ports, packet floods, or unauthorized access
* Apply custom filters for traffic isolation
* Document findings for future replication or SOC use

---

## 🧰 Tools Used

* **Wireshark** – Deep packet inspection and network filtering
* **Microsoft SysInternals** – System monitoring utilities (e.g., TCPView, Process Monitor)

---

## 📁 Project Structure

```
Intrusion-Detection/
├── packet-captures/               # Raw and filtered .pcap files
├── wireshark-filters.txt          # Custom filters used during analysis
├── sysinternals-logs/             # System event logs from test VM
├── summary-report.pdf             # 2-page incident summary (findings + actions)
└── README.md                      # Project overview and usage
```

---

## 🛠️ Methodology

1. **Simulated suspicious behavior** (e.g., port scans, failed logins, file transfers)
2. Captured traffic using **Wireshark** while SysInternals tracked system behavior
3. Applied **5+ custom filters** to isolate signs of malicious activity
4. Identified anomalies (e.g., repeated SYN packets, unrecognized protocols)
5. Summarized results in a structured incident report

---

## 🔐 Sample Filters Used

```plaintext
tcp.flags.syn == 1 && tcp.flags.ack == 0        # SYN flood detection
http.request.method == "POST"                   # Suspicious data upload
frame.len > 1000                                # Oversized payloads
ip.addr == 192.168.1.103                        # Isolate attacker host
```

---

## 📊 Results

* Detected **3 categories** of anomalous behavior:

  * TCP SYN floods
  * Suspicious HTTP POST uploads
  * Communication on non-standard ports
* Achieved **high alert precision** by combining host-based and packet-level analysis
* Created a **replicable analysis framework** for future IDS testing

---

## 🚀 Future Improvements

* Integrate alerts into a centralized SIEM (e.g., Wazuh or Splunk)
* Add rule-based alerts using Snort or Suricata
* Expand coverage to include DNS tunneling and malware callbacks

---

## 📞 Contact

**Mark Ford Jr.**
GitHub: [markfordjr](https://github.com/markfordjr)
Project Repo: [Intrusion Detection](https://github.com/markfordjr/Intrusion-Detection)

---

## 📄 License

Open-sourced under the [MIT License](LICENSE)
