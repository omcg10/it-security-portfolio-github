# Remediation & Hardening

## Disable Telnet Service

```bash
sudo systemctl stop telnet.socket
sudo systemctl disable telnet.socket
```

or

```bash
sudo apt purge telnetd
```

## Enforce Password Change

```bash
sudo passwd admin
```

## Recommended Replacement (SSH)

```bash
sudo apt install openssh-server
sudo systemctl enable ssh
sudo systemctl start ssh
```

## Verification Scan

```bash
nmap -p 23 192.168.107.129
```

**Expected Result**
- Port 23 closed
