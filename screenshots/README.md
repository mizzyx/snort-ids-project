# Snort IDS Project

## Overview

This project demonstrates a basic Intrusion Detection System (IDS) using Snort.

Kali Linux was used to generate controlled network traffic, while Ubuntu Linux was used to monitor and analyze the traffic using Snort.

## Lab Environment

- Traffic Generator: Kali Linux
- IDS / Monitoring System: Ubuntu Linux
- IDS Software: Snort
- Network Interface: enp0s3

## Network Testing

Controlled network traffic was generated from Kali Linux for testing:

- ICMP ping traffic
- Nmap scanning traffic
- Hping-generated traffic

The traffic was sent toward the Ubuntu monitoring system.

## Snort Detection

Snort was configured with custom detection rules stored in:

`rules/local.rules`

The generated traffic was monitored on Ubuntu and Snort was used to detect suspicious network activity and generate alerts.

## Evidence

Screenshots of the testing process are available in the [`screenshots`](screenshots/) directory.

### Traffic Generation

Kali Linux screenshots document:

- ICMP ping testing
- Nmap scanning
- Hping-generated traffic

### Traffic Detection

Ubuntu screenshots document Snort monitoring and detecting the generated traffic.

## Project Structure

```text
snort-ids-project/
├── rules/
│   └── local.rules
├── screenshots/
│   ├── README.md
│   ├── ping.png
│   ├── nmap.png
│   ├── hping.png
│   └── snort-ubuntu-alerts.png
└── README.md
