# Methodology & Commands

## Phase 1 – Enumeration

### Service & OS Discovery
```bash
nmap -sV -O 192.168.107.129
```

**What this checks**
- Open ports
- Running services
- OS fingerprinting

**Result**
- Port 23 (Telnet) open
- Linux kernel detected (3.x / 4.x)

---

## Phase 2 – Exploitation Testing

### Telnet Login Test
```bash
telnet 192.168.107.129
login: admin
password: admin
```

**Result**
- Successful login
- Low-privilege shell access

⚠️ This confirms insecure default credentials.
