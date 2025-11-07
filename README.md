# ufw_configuration.sh

# 🔥 Basic Firewall Configuration with UFW

## 🧭 Objective
To set up and configure a *basic firewall* on a Linux system using *UFW (Uncomplicated Firewall)* and to control network traffic by allowing or denying specific ports.

---

## 🧰 Tools Used
- *Operating System:* Ubuntu (or any Debian-based Linux)
- *Firewall Utility:* UFW (Uncomplicated Firewall)
- *Privileges:* Root or sudo access

---

## ⚙ Steps Performed

### *1. Install UFW*
First, update your system and install UFW:
```bash
sudo apt update
sudo apt install ufw -y
ufw --version
sudo ufw enable
sudo ufw status verbose
sudo ufw allow ssh
sudo ufw deny http
sudo ufw status numbered
Status: active

To                         Action      From
--                         ------      ----
22/tcp                     ALLOW       Anywhere
80/tcp                     DENY        Anywhere
22/tcp (v6)                ALLOW       Anywhere (v6)
80/tcp (v6)                DENY        Anywhere (v6)
