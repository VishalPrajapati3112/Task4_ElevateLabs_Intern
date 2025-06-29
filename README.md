
Setup and Use a Firewall on Windows/Linux

# 🔐 Task 4 - Linux Firewall Configuration using UFW

## 🎯 Objective
To configure and test basic firewall rules using UFW on Kali Linux and verify secure remote access through SSH.

## 🧰 Environment
- OS: Kali Linux (VirtualBox)
- Tool: UFW (Uncomplicated Firewall)
- Remote Access Test: From Windows CMD via SSH

## 🛠 Steps Performed
1. Installed and enabled UFW:
   ```bash
   sudo apt update
   sudo apt install ufw
   sudo ufw enable
   ```

2. Allowed SSH access (port 22):
   ```bash
   sudo ufw allow 22
   ```

3. Blocked insecure Telnet port (port 23):
   ```bash
   sudo ufw deny 23
   ```

4. Verified active rules:
   ```bash
   sudo ufw status numbered
   ```

5. SSH tested from Windows CMD:
   ```bash
   ssh username@<Kali-IP>
   ```

6. Removed test rule after verification:
   ```bash
   sudo ufw delete deny 23
   ```

## 📸 Screenshot
- Screenshot included in the repository.

## 🧠 Key Learnings
- UFW helps manage iptables easily
- Firewalls filter traffic using port-based rules
- Importance of allowing essential services like SSH
- Telnet should be blocked as it is insecure



