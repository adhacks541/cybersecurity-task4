# 🔐 Task 4: Setup and Use a Firewall on Linux

## 🎯 Objective
Configure and test basic firewall rules using UFW (Uncomplicated Firewall) on a Linux machine to understand how network traffic filtering works.

---

## 🛠 Tools Used
- **Operating System**: Ubuntu 22.04 (or any Debian-based Linux)
- **Firewall Utility**: UFW (Uncomplicated Firewall)

---

## ✅ Steps Performed

1. Installed UFW
sudo apt update
sudo apt install ufw -y
2. Enabled the Firewall

sudo ufw enable

3. Checked Current Rules

sudo ufw status numbered

4. Blocked Inbound Traffic on Port 23 (Telnet)

sudo ufw deny 23

5. Allowed SSH (Port 22)

sudo ufw allow 22

6. Verified Rules Applied

sudo ufw status verbose

7. Deleted Test Rule for Port 23

sudo ufw delete deny 23

📸 Screenshots

All screenshots of terminal outputs and command usage are available.
🧠 Summary: How UFW Filters Traffic

    UFW simplifies firewall rule creation by using easy syntax to allow or deny ports/services.

    Rules are applied based on direction (inbound/outbound) and interface.

    Blocking port 23 (Telnet) is recommended as Telnet transmits data in plaintext and is insecure.

    Allowing port 22 (SSH) ensures remote access is not interrupted.

📁 Deliverables

    UFW command output screenshots

    ufw-status.txt showing active firewall rules

    This README.md file
