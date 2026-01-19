# Day 4 – SSH Hardening and Authentication Detection

## Objective
The objective of Day 4 was to harden SSH access on a Linux server by enforcing key-based authentication, disabling insecure access methods, and validating detection capabilities through authentication log analysis. This work focuses on reducing attack surface and ensuring authentication events are auditable for SOC monitoring.

---

## Environment
- **Host OS:** macOS
- **Virtualization:** UTM
- **Guest OS:** Ubuntu Server 24.04 LTS (aarch64)
- **Role:** SOC analyst / systems hardening
- **Network:** Private VM network (192.168.64.0/24)

---

## SSH Hardening

### Key-Based Authentication
An ED25519 SSH key pair was generated on the client machine and deployed to the server.

- Private key stored securely on the client
- Public key added to the server user’s `~/.ssh/authorized_keys`
- SSH agent used for key management on macOS

**Result:**
- Passwords are no longer required for authentication
- Login succeeds only when a valid private key is presented

---

### SSH Server Configuration
The SSH daemon was hardened by explicitly setting the following parameters in `/etc/ssh/sshd_config`:

```text
PasswordAuthentication no
PubkeyAuthentication yes
KbdInteractiveAuthentication no
PermitRootLogin no
