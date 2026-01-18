# Day 3 – Security Baseline & Access Control

## System Setup
- Ubuntu Server 24.04 LTS
- UTM virtualization on macOS
- CLI-only administration

## Network
- Interface: enp0s1
- Private IP: 192.168.64.2

## Firewall (UFW)
- Default deny incoming
- Allowed service: OpenSSH
- Firewall enabled at boot

## Authentication Events Observed
- Failed SSH login attempt
- Successful SSH login
- Privilege escalation via sudo
- Commands fully logged in auth.log

## Logs Analyzed
- /var/log/auth.log

## Security Takeaways
- Authentication failures are logged and traceable
- Privilege escalation events are auditable
- Firewall rules must be defined before activation

