# Intrusion Detection - Term Project

Overview

This project focuses on intrusion detection techniques and the analysis of a persistent backdoor attack. The objective was to deploy, detect, and analyze a backdoor in a controlled lab environment using Kali Linux and Windows VM. The project documentation includes task descriptions and screenshots to validate completion.

Features

Persistent Backdoor Deployment  
Created a backdoor that persists across system reboots.
Configured the backdoor to run automatically at startup.
Used netcat (nc) in Kali Linux to establish a reverse shell connection to the Windows VM.

Intrusion Detection Techniques  
Network Traffic Analysis using Wireshark to identify unusual communication patterns.
Startup Program Inspection using Autoruns to detect unauthorized startup processes.
Windows Event Logs to analyze potential security alerts related to the backdoor execution.

Screenshots

The report includes screenshots demonstrating:
Creation of the persistent backdoor.
Successful exploitation via netcat.
Detection using Wireshark, Autoruns, and Windows Logs.

Tools Used

Kali Linux: For deploying the backdoor and performing network analysis.
Windows VM: Target system for exploitation and detection.
Wireshark: For monitoring and detecting suspicious network traffic.
Autoruns (Sysinternals): For identifying unauthorized startup programs.
Windows Event Viewer: For log analysis and intrusion detection.

How to Use This Project

This project serves as a demonstration of intrusion detection techniques for cybersecurity professionals and students. It can be used to:

Understand how persistent backdoors are deployed.
Identify key indicators of compromise (IoCs).
Analyze logs and traffic for forensic investigation.
Author
This project was completed as part of a cybersecurity term assignment, focusing on digital forensics and intrusion detection.
