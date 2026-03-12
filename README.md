# Basic-Keylogger
# 🔐 Basic Keylogger Lab

A simple **educational cybersecurity project** demonstrating how a basic keylogger works in a controlled virtual lab environment using **Kali Linux (attacker)** and **Ubuntu/SEED (victim)**.

This project is strictly for **educational and ethical cybersecurity learning purposes only**.

---

# Project Overview

This project simulates a **keylogging attack scenario** to demonstrate how attackers capture keystrokes and send them to a remote server.

The lab environment consists of two virtual machines:

- **Kali Linux** → Attacker machine (receives keystrokes)
- **Ubuntu / SEED Ubuntu** → Victim machine (runs keylogger)

Captured keystrokes are sent using **HTTP POST requests** and stored on the attacker machine.

---

# Lab Architecture

```
Ubuntu (Victim)            Kali Linux (Attacker)
10.0.2.4  ─────HTTP POST───▶ 10.0.2.3:8080
     Keylogger                   Listener Server
```

Workflow:

1. Victim captures keyboard input
2. Keystrokes are stored in a buffer
3. Data is sent to attacker using HTTP
4. Attacker server prints and stores the logs

---

# Cybersecurity Concepts Demonstrated

This project demonstrates several important security concepts:

- Keylogging
- Data exfiltration
- HTTP command & control communication
- Malware behavior analysis
- Network traffic monitoring

# Author
Cybersecurity Learning Project  
GitHub: https://github.com/SHELLY1209
