# soc-home-lab
# SOC Home Lab

This repository documents the design and implementation of a Linux-based Security Operations Center (SOC) home lab built using virtual machines on macOS.

The goal of this project is to develop a strong understanding of Linux systems, networking, and secure software behavior through hands-on experimentation in a controlled environment.

---

## Project Goals
- Understand Linux process behavior and system logging
- Build a centralized monitoring system (SOC)
- Collect and analyze system telemetry
- Simulate security-relevant events safely
- Document system behavior and detections like a real engineer

## Project Progress

### Day 1 – Environment Setup
- Created GitHub repository
- Defined SOC lab architecture and goals
- Set up Ubuntu Server VM using UTM on macOS

### Day 2 – OS Installation & Networking
- Installed Ubuntu Server 24.04 LTS
- Configured network interface and DHCP
- Created administrative user with sudo privileges
- Enabled OpenSSH

### Day 3 – Security Baseline
- Enabled and configured UFW firewall
- Verified SSH access
- Reviewed authentication and sudo logs
- Observed failed and successful login events
- Documented security baseline and audit logs---

## Lab Architecture
- **Host:** macOS
- **SOC Server:** Ubuntu Server (log collection and analysis)
- **Endpoint:** Ubuntu Desktop (monitored system)
- **Test System:** Kali Linux (controlled testing)

---

## Project Status
**Day 1 – Infrastructure and Linux fundamentals**

Further components (monitoring, detections, and analysis) will be added incrementally.
