# Findings Breakdown

## 1. Default Credentials (Critical)

**Issue**
- Username: admin
- Password: admin

**Impact**
- Immediate unauthorized access
- No brute force required

**Why this matters in IT**
- Common misconfiguration in legacy systems
- Often exploited during internal audits

---

## 2. Telnet Enabled (High)

**Issue**
- Cleartext authentication
- Credentials exposed over the network

**Command Evidence**
```bash
nmap -p 23 192.168.107.129
```

**IT Perspective**
- Violates basic security baselines
- SSH should always replace Telnet

---

## 3. End-of-Life Operating System (High)

**Issue**
- Kernel no longer supported
- Known CVEs likely present

**Why this matters**
- No security patches
- Compliance and audit failure risk
