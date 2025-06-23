# 🔍 Nmap Network Scanning Guide

This project provides a quick and practical guide for performing local network scans using [Nmap](https://nmap.org/). It is intended for cybersecurity beginners, ethical hackers, or anyone interested in understanding network visibility and basic threat surface analysis.

---

## 📦 Requirements

- [Nmap](https://nmap.org/download.html)
- (Optional) [Wireshark](https://www.wireshark.org/) for packet analysis
- Basic understanding of IP addressing and ports

---

## 🚀 Quick Start

1. **Install Nmap**
   - Download and install from: https://nmap.org/download.html
   - Linux: `sudo apt install nmap`  
   - macOS: `brew install nmap`

2. **Find Local IP Range**
   - Run `ipconfig` (Windows) or `ip a` (Linux/macOS)
   - Note your IP (e.g., `192.168.1.105`) and deduce the subnet (`192.168.1.0/24`)

3. **Perform a TCP SYN Scan**
   ```bash
   nmap -sS 192.168.1.0/24

## Note IP Addresses and Open Ports

- Look for active hosts and services running on common ports.

## (Optional) Analyze Packets in Wireshark

- Start a capture while running your scan.

- Filter by IP or port using Wireshark display filters.

## Save Scan Results

- nmap -sS 192.168.1.0/24 -oN scan_results.txt

