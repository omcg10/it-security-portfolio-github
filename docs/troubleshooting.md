# Troubleshooting & Validation

## Telnet Still Showing as Open?
- Ensure service is stopped
- Check inetd / xinetd
```bash
sudo systemctl status openbsd-inetd
```

## SSH Not Accessible?
- Check firewall rules
```bash
sudo ufw status
```

- Verify SSH service
```bash
systemctl status ssh
```

## Nmap Shows OS Guess Wrong?
- Use aggressive scan
```bash
nmap -A 192.168.107.129
```
