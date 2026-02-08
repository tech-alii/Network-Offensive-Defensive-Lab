# MAC Flooding Attack

## 📌 Overview
This project focuses exclusively on the **MAC Flooding attack**, a Layer 2
network attack that targets the CAM (Content Addressable Memory) table of a
switch.
The objective is to study how this attack works, its impact on network behavior,
and why securing Layer 2 infrastructure is critical.

---

## 🎯 Objectives
- Understand how switches learn MAC addresses
- Explain the role of the CAM table
- Analyze how CAM table overflow occurs
- Study the security impact of MAC Flooding
- Identify effective mitigation techniques

---

## 🧪 Lab Environment
The experiment was conducted in a controlled laboratory environment using:

- GNS3
- Kali Linux (Attacker)
- Ubuntu Linux (Victim)
- Layer 2 Switch
- Router (Gateway)

⚠️ No real or production networks were involved.

---

## 🧠 Attack Description
A switch maintains a CAM table to map MAC addresses to physical ports.
In a MAC Flooding attack, the attacker sends a high volume of Ethernet frames
with **spoofed source MAC addresses**.

As the CAM table fills up:
- The switch is unable to learn new MAC addresses
- Legitimate MAC entries may be overwritten
- Frames are broadcast to all switch ports

This causes the switch to behave like a **hub**, breaking traffic isolation.

---

## ⚠️ Impact
- Degradation of switch performance
- Increased broadcast traffic
- Loss of traffic confidentiality
- Network instability
- Enables further Layer 2 attacks

---

## 🛡️ Defense & Mitigation
The following security measures are effective against MAC Flooding:

- Port Security (MAC address limiting)
- Static MAC address configuration
- Disabling unused switch ports
- Network monitoring and alerting
- VLAN segmentation

Proper configuration of **Port Security** effectively prevents this attack.

---

## 🧠 Expert Insight
MAC Flooding is rarely used as a standalone attack.
Its primary purpose is to weaken Layer 2 security and enable traffic interception
and more advanced attacks.

This highlights the importance of securing network infrastructure at the
switch level.

---

## ⚖️ Legal Disclaimer
This project is intended strictly for **educational purposes**.
All activities were performed in a closed laboratory environment.
Any unauthorized use of these techniques on real networks is illegal.

---

## 📚 Educational Context
This project is part of a Network Security lab for students studying
Networks and Systems (Réseaux et Systèmes) and cybersecurity fundamentals.

---
