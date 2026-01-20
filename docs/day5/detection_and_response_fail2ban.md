# Day 5 – Detection and Automated Response (Fail2Ban)

## Objective
Implement host-based intrusion detection and automated response to protect the SOC server from brute-force SSH attacks.

---

## Environment
- Ubuntu Server 24.04 LTS
- OpenSSH
- UFW Firewall
- Fail2Ban
- systemd

---

## Threat Model
The primary threat addressed is brute-force SSH authentication attempts originating from unauthorized hosts.

---

## Detection Mechanism

Fail2Ban monitors authentication logs to detect repeated SSH failures.

Monitored log file:
- `/var/log/auth.log`

Fail2Ban parses this log in real time to identify:
- Failed SSH login attempts
- Repeated authentication failures from the same IP

---

## Automated Response

When the failure threshold is exceeded:
- The offending IP is automatically banned
- Firewall rules are applied dynamically
- SSH access from the source is blocked

This response is temporary and expires automatically after a configured duration.

---

## Validation Steps

Fail2Ban service status:

```bash
systemctl status fail2ban
