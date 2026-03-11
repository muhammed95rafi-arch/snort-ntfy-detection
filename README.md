# snort-ntfy-detection
Real-time Nmap Scan Detection Using Snort IDS With Ntfy Alert Notification


# Snort - Ntfy Detection (Real-Time Nmap Scan Alert)

## Overview
This project demonstrates real-time detection of Nmap port scanning attacks using Snort IDS and sending instant alerts through ntfy notification service.

When a scan is performed using Nmap, Snort detects the activity and a script automatically sends a notification to the ntfy server.

## Tools Used
- Snort IDS
- ntfy notification service
- Nmap
- Ubuntu Server 22.04
- Windows 11
- VMware Workstation

## Lab Setup

Monitoring System
Ubuntu Server 22.04  
Tool: Snort + ntfy  
IP Address: 192.168.222.133

Attack Machine
Windows 11  
Tool: Nmap

Network
192.168.222.0/24 (VMware private network)

## How It Works
1. Snort monitors network traffic.
2. When an Nmap scan is detected, Snort generates an alert.
3. The alert is written to the Snort log file.
4. A bash script reads the log file.
5. The script sends a notification to the ntfy server.

## Example Alert
NMAP TCP Scan Detected  
Source IP: 192.168.222.1  
Destination IP: 192.168.222.133
https://drive.google.com/file/d/1G3Zj-gSMXPl3oe-y-wKEZ1EfNXDFslGG/view?usp=drive_link


## Purpose
The goal of this project is to demonstrate basic SOC monitoring workflow by detecting reconnaissance activity and generating real-time alerts.

## Disclaimer
This project was performed in a controlled lab environment for educational purposes only.
