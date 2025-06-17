# Network-Based Attack Detection Using UFW Logs

This project demonstrates how to simulate a basic HTTP port scan attack using **Nmap** from a Kali Linux machine and detect it using **UFW logs** on an Ubuntu target system.

---

## Objective

To simulate a network-based reconnaissance attempt and analyze how **UFW (`Uncomplicated Firewall`)** logs can help detect early-stage scanning behavior — a common tactic in cyber attacks.

---

## 🖥️ Lab Environment

| Role        | OS           | Tools Used           |
|-------------|--------------|----------------------|
| Attacker    | Kali Linux   | `nmap`               |
| Target      | Ubuntu Linux | `ufw`, `/var/log/ufw.log` |

---

## Attack Simulation – Port Scan

On the **attacker machine (Kali Linux)**:

```bash
nmap -p80 <TARGET-IP>
