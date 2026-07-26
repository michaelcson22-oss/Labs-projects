# Home Network Infrastructure Lab

## Overview

This project documents the design, configuration, and management of my home network laboratory. The lab was built to develop practical networking skills by configuring enterprise-style networking concepts in a real environment.

The network supports multiple wired and wireless devices while providing a platform for learning network administration, troubleshooting, monitoring, and security.

---

# Objectives

- Design a secure and reliable home network
- Configure router and switch settings
- Understand DHCP and DNS functionality
- Practice network troubleshooting
- Improve Wi-Fi performance and coverage
- Monitor network traffic
- Build a foundation for enterprise networking concepts

---

# Network Environment

| Component | Details |
|-----------|---------|
| ISP | AT&T Fiber 1000 Mbps |
| Gateway | AT&T BGW320-500 |
| Router | TP-Link Archer AXE5400 (Wi-Fi 6E) |
| Switch | TP-Link TL-SG2008 Managed Switch |
| Desktop | Windows 11 |
| Wireless Devices | Laptop, Smartphone, Smart TV, Gaming Console |
| Management Software | TP-Link Omada |

---

# Network Topology

--
                          Internet
                              │
                       AT&T Fiber (1 Gbps)
                              │
                     BGW320-500 Gateway
                              │
                 TP-Link Archer AXE5400 Router
                              │
          ┌───────────────────┴───────────────────┐
          │                                       │
   TP-Link TL-SG2008                      Wireless Clients
    Managed Switch                                │
          │                                       ├── iPhone 15
   ┌──────┼───────────────┐                       ├── iPhone
   │      │               │                       └── Laptop
   │      │               │
Windows 11 PC         PlayStation 5
                      PlayStation 5
--

---

# Technologies Used

- TCP/IP
- DHCP
- DNS
- NAT
- IPv4
- Wi-Fi 6E
- Ethernet
- Managed Switching
- VLAN Fundamentals
- Network Monitoring
- Windows Networking

---

# Hardware

## Router

- TP-Link Archer AXE5400
- Wi-Fi 6E
- Dual-band / Tri-band wireless
- DHCP Server
- NAT
- Port Forwarding
- QoS
- WPA3 Security

---

## Managed Switch

- TP-Link TL-SG2008
- Gigabit Ethernet
- Web Management
- VLAN Support
- Port Monitoring
- Network Diagnostics

---

# Configuration Tasks

## Network Configuration

✔ Configured router

✔ Configured wireless networks

✔ Updated firmware

✔ Configured DHCP

✔ Reserved IP addresses for important devices

✔ Verified internet connectivity

---

## Wireless Configuration

Configured:

- WPA2/WPA3 Security
- SSID Management
- Wi-Fi Channel Selection
- Device Connectivity
- Signal Optimization

---

## DHCP

Configured:

- DHCP Address Pool
- Reserved IP Addresses
- Lease Management
- Default Gateway
- DNS Server Assignment

---

## DNS

Learned and verified:

- Public DNS
- Local DNS
- Name Resolution
- DNS Troubleshooting

---

## Network Monitoring

Performed:

- Ping Testing
- Traceroute
- IP Configuration Review
- DNS Testing
- Packet Capture with Wireshark

---

## Windows Networking

Practiced using:

- ipconfig
- ping
- tracert
- nslookup
- netstat

---

# Skills Demonstrated

- Network Troubleshooting
- Router Administration
- Managed Switch Administration
- DHCP Configuration
- DNS Fundamentals
- Wireless Networking
- Windows Networking
- Command Line Networking
- Documentation
- Problem Solving

---

# Troubleshooting Scenarios

Examples of issues investigated:

- Slow wireless performance
- DNS resolution failures
- IP addressing conflicts
- Internet connectivity issues
- DHCP lease problems
- Device connectivity
- Wi-Fi signal optimization

---

# Security

Implemented:

- WPA3 Wireless Security
- Strong Administrative Passwords
- Firmware Updates
- Guest Network Configuration
- Disabled unused features
- Network segmentation research

---

# Screenshots

Include screenshots of:

- Router Dashboard
- Managed Switch Dashboard
- DHCP Configuration
- Client List
- Speed Tests
- Wireshark Packet Capture
- Windows Network Settings
- Command Prompt Network Commands

---

# Lessons Learned

Building this lab strengthened my understanding of how routers, switches, DHCP, DNS, and wireless networking work together in a real environment. It also improved my troubleshooting methodology by requiring systematic testing of connectivity, IP configuration, and network performance.

---

# Future Improvements

- Configure VLANs
- Build a pfSense firewall lab
- Deploy a Windows Server VM
- Implement network monitoring with PRTG
- Configure VPN access
- Learn IPv6 administration
- Deploy Microsoft Entra-connected devices
- Add a NAS for centralized storage
