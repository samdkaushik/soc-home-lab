# SOC Home Lab

## Overview

This repository documents the design and implementation of a Linux-based **Security Operations Center (SOC) Home Lab** built using virtual machines on macOS. The lab is designed to provide hands-on experience with Linux system administration, secure access control, logging, and security monitoring in a controlled environment.

The project emphasizes operating systems fundamentals, networking, authentication, auditing, and defensive security practices commonly used in enterprise environments.

---

## Objectives

- Develop practical Linux system administration skills
- Understand authentication, authorization, and privilege escalation
- Configure secure remote access using SSH
- Implement host-based firewall controls
- Analyze system and authentication logs
- Simulate and observe security-relevant events safely
- Document findings and configurations like a real SOC engineer

---

## Lab Environment

- **Host OS:** macOS  
- **Virtualization:** UTM  
- **Guest OS:** Ubuntu Server 24.04 LTS  
- **Interface:** CLI-only (no GUI)  
- **Networking:** NAT / private subnet  

---

## Repository Structure

## Progress Summary

### Day 1 – Environment & Repository Setup
- Created GitHub repository
- Defined project goals and SOC lab scope
- Designed initial directory structure
- Set up Ubuntu Server VM using UTM

### Day 2 – OS Installation & Networking
- Installed Ubuntu Server 24.04 LTS
- Configured network interface with DHCP
- Created administrative user with sudo privileges
- Installed and enabled OpenSSH

### Day 3 – Security Baseline & Access Control
- Enabled and configured UFW firewall
- Allowed SSH access before firewall activation
- Verified firewall persistence across reboots
- Reviewed authentication logs (`/var/log/auth.log`)
- Observed failed and successful SSH login attempts
- Analyzed privilege escalation events via sudo
- Documented findings and security takeaways

---

## Key Concepts Demonstrated

- Linux user and privilege management
- Secure remote access (SSH)
- Firewall configuration (UFW)
- Authentication and authorization logging
- Audit trails and system observability
- Command-line–only system administration
- Professional documentation practices

---

## Security Notes

- Password-based SSH access is currently enabled for initial setup
- SSH hardening and key-based authentication will be implemented in later stages
- Log monitoring and intrusion prevention mechanisms will be added incrementally

---

## Author

Samarth Kaushik
