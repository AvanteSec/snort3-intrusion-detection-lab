# snort3-intrusion-detection-lab
A hands-on cybersecurity lab implementing Snort 3 IDS in a VirtualBox environment to monitor network traffic and detect potential threats.

## Project Overview

The purpose of this project is to build a virtual cybersecurity lab using Oracle VirtualBox and configure Snort 3 as a Network Intrusion Detection System (NIDS).

This lab allows me to practice network monitoring, packet analysis, and creating custom detection rules in a controlled environment.

I installed Snort 3.12.2.0 from source on Ubuntu Linux and configured a custom rule to detect ICMP echo requests generated from Kali Linux.

**Project Status:** In Progress

### Project Objectives

- Configure an isolated virtual network for cybersecurity testing.
- Install and configure Snort 3 on Ubuntu Linux.
- Generate network traffic using Kali Linux.
- Develop custom Snort detection rules.
- Analyze network packets and investigate security alerts.
- Document troubleshooting challenges and solutions.

## Lab Environment

This project uses Oracle VirtualBox to create a virtualized cybersecurity testing environment.

### Virtual Machines

| Virtual Machine | Purpose |
|---|---|
| Ubuntu Linux | Hosts Snort 3 and monitors network traffic |
| Kali Linux | Generates network traffic for testing detection rules |
| Metasploitable | Provides a vulnerable target for future security testing |

### Network Configuration

The Ubuntu and Kali Linux virtual machines communicate over a virtual network.

- **Ubuntu IP Address:** `172.30.1.23`
- **Kali Linux IP Address:** `172.30.1.20`
- **Ubuntu Monitoring Interface:** `enp0s8`

I verified connectivity between Kali Linux and Ubuntu using ICMP echo requests (ping). I also used `tcpdump` on Ubuntu to confirm that ICMP packets were reaching the monitoring interface.

### Tools and Technologies

- Oracle VirtualBox
- Ubuntu Linux
- Kali Linux
- Snort 3.12.2.0
- LibDAQ
- tcpdump
- Linux command-line utilities
