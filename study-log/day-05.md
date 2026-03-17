# CPTS Preparation – Day 05

Date: March 16, 2026

## Study Time

HTB Academy Study: 1h 03m  
Lab Practice: 3h 43m  

Total Study Time: ~4h 46m

---

# Topics Covered

Today was a productive day with **four focused study sessions**, combining hands-on lab practice with theoretical learning on HTB Academy.

The main focus of the day was **reinforcing exploitation techniques and practicing service enumeration**.

---

# Lab Practice

## Machine Revisited – DocFlow

Today I revisited the **DocFlow** machine and solved it again to reinforce my understanding of the exploitation process.

Re-solving the machine helped me:

- reinforce the attack path
- better understand the vulnerability chain
- improve the speed of exploitation

By repeating the machine, the entire process became much clearer and easier to reproduce.

---

## Machine Completed – Saori

I also solved the **Saori** machine today.

During this machine I practiced several skills including:

- network traffic analysis with **Wireshark**
- subdomain discovery
- HTTP authentication analysis
- Base64 credential decoding
- SSH access
- Linux privilege escalation
- Ghostscript sandbox escape
- CVE exploitation

Final Result:

```
User: root
System: Linux
Platform: HackingClub
Machine: Saori
Difficulty: Easy
```

The machine was successfully compromised.

---

# Additional Skills Practiced

While working on **DocFlow**, I also practiced and reviewed the following techniques:

- Nmap reconnaissance
- web directory enumeration
- dependency vulnerability analysis
- JWT token manipulation
- webpack source map analysis
- remote code execution through vulnerable libraries
- reverse shell techniques
- shell stabilization
- command injection exploitation
- Linux privilege escalation
- disk group abuse
- SSH private key extraction

Revisiting these techniques helped reinforce my understanding of the full exploitation process.

---

# HTB Academy Study

In the evening session, I continued studying the **Offensive – Getting Started** module.

Today's focus was on **service scanning and enumeration**.

---

# Service Scanning with Nmap

I studied how **Nmap** can be used to identify open ports and running services on a target system.

This includes discovering:

- open ports
- service versions
- potential entry points

Understanding service discovery is a fundamental step during **reconnaissance and enumeration**.

---

# Common Network Services

The module introduced two important services frequently encountered during penetration testing.

## FTP (File Transfer Protocol)

FTP is commonly used for file transfers between systems.

Misconfigured FTP servers may allow:

- anonymous login
- access to sensitive files
- information disclosure

---

## SMB (Server Message Block)

SMB is commonly used for **file sharing in Windows environments**.

Misconfigured SMB services can allow attackers to:

- enumerate shares
- access sensitive files
- gather credentials
- discover internal system information

---

# Practical Exercises

Two practical exercises required connecting to HTB lab machines using the **Parrot OS environment**.

During these exercises I had to:

- perform **Nmap scans**
- enumerate network services
- retrieve flags from the target machines
- interact with services using **Netcat**
- perform **banner grabbing** to identify running services

These exercises reinforced how enumeration tools are used in real attack scenarios.

---

# Progress Update

Today I continued progressing through the CPTS path.

Current completion progress: **4%**

---

# Reflection

Today was a very productive study day with **four focused sessions**.

The combination of:

- repeating previously solved machines
- solving new lab machines
- studying service enumeration techniques

helped reinforce both **practical exploitation skills and theoretical knowledge**.

Revisiting machines such as **DocFlow** made the attack chain easier to understand, while solving **Saori** introduced new concepts and vulnerabilities.

The concepts covered today, especially **Nmap scanning, SMB enumeration, and banner grabbing**, are fundamental techniques that will be used repeatedly in future penetration testing scenarios.