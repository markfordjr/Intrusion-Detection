# 🛡️ Intrusion Detection: Persistent Backdoor Detection (Digital Forensics Project)

This project simulates a real-world persistent backdoor attack and demonstrates how intrusion detection tools can be used to identify and analyze the compromise. It was completed as part of a Digital Forensics course, focused on understanding adversary persistence mechanisms and defensive detection strategies.

## 🔍 Objective
- Deploy a persistent backdoor using `nc` (Netcat) between Kali Linux and a Windows VM
- Establish reverse shell access from the attacker (Kali) to the target (Windows)
- Detect and analyze the backdoor activity using Wireshark and SysInternals' Autoruns

## 🧰 Tools Used
- Kali Linux (Attacker VM)
- Windows 10 VM (Target)
- Netcat (nc)
- Wireshark
- Microsoft SysInternals Autoruns
- Windows Logs/Event Viewer

## 💡 Key Takeaways
- Demonstrated backdoor persistence via startup folder
- Identified unusual periodic network traffic using Wireshark
- Detected unauthorized autorun activity using SysInternals
- Reinforced importance of endpoint visibility and log correlation

## 📸 Screenshots
- Backdoor persistence in Windows startup
- Netcat session from Kali to Windows
- Wireshark traffic showing suspicious behavior
- Autoruns showing unauthorized programs at startup

## 📚 Course
Digital Forensics – University of Massachusetts Lowell  
Term Project – 2025
