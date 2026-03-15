# Phase 2: Security Hardening & Logging

This phase focuses on implementing host-based security controls and generating security telemetry that can later be ingested into a SIEM platform.
The goal is to simulate how security engineers harden systems and produce logs that SOC analysts use for detection and investigation.

---

# Phase Objectives

• Enable detailed security logging on Windows systems  
• Implement host-based firewall controls on Linux servers  
• Simulate authentication failures and suspicious activity  
• Analyze system logs to understand how security events are recorded  

---

# Lab Environment

- Ubuntu Server -> Domain Controller (Samba AD)
- Ubuntu Server -> SIEM Server
- Windows 11 ARM -> Domain Workstation
- Kali Linux -> Attacker Machine

Internal Lab Network:
- 192.168.200.0/24
- Domain Controller -> 192.168.200.10 
- SIEM Server -> 192.168.200.20 
- Windows Client -> 192.168.200.30 

---

# Focus Areas

## Windows Advanced Audit Policies
 
Advanced audit policies are enabled to capture authentication activity, privilege usage, and process execution.

---

## Linux Firewall Configuration

A host-based firewall is implemented using **UFW (Uncomplicated Firewall)**.

The firewall enforces a **default deny inbound policy**, meaning only explicitly permitted services are accessible.

This reduces the attack surface by restricting network exposure to only necessary services.

---

## Authentication Failure Simulations

Controlled authentication failures will be generated in order to produce realistic security events. These events allow analysis of how authentication failures appear in system logs.

---

## Log Analysis and Event Review

Security logs from both Windows and Linux systems will be analyzed to build familiarity with raw log analysis before centralized logging is introduced.

---

# Phase Outcome

At the end of this phase the lab environment will have:

• hardened hosts  
• detailed security logging enabled  
• authentication telemetry generated  
• security events ready for SIEM ingestion  

These logs will later be centralized and analyzed during **Phase 3 – SIEM Deployment**.
