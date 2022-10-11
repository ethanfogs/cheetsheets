# MACOS COMMAND-LINE CHEATSHEET

---

## NETWORKING COMMANDS

### HOSTNAME
```bash
sudo scutil --set HostName <name>
sudo scutil --set Computername <name>
sudo scutil --set LocalHostName <name>
```

### SSH
- Reloading sshd_config
```bash
sudo visudo /etc/ssh/sshd_config
sudo launchctl stop com.openssh.ssh-agent # will auto-restart ssh daemon
```

---

### DNS
- Modify DNS server(s)
```bash
sudo networksetup -setdnsservers <net-iface(usually `en0`)> <dns [hostname|ip]>
```
