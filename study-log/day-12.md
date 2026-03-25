# CWES Preparation – Day 12

Date: March 23, 2026

## Study Time

CWES Preparation (HTB Academy): 1h 16m  
Web Practice (PortSwigger Labs): 1h 05m  
Bug Bounty Practice: 24m  
Lab Practice: 44m  

Total Study Time: ~3h 30m

---

# Topics Covered

Today I focused on **API interaction, authentication flaws, and tooling limitations**, along with hands-on system troubleshooting in Linux.

---

# HTB Academy Study (CWES Path)

## Module Completed

- Web Requests (final section)

---

## Key Concepts Studied

- interacting with APIs using **cURL**
- performing CRUD operations through HTTP requests
- understanding how APIs handle user input and authentication
- manipulating requests outside of the browser

This reinforced how attackers can interact directly with backend systems.

---

# Web Practice – PortSwigger Lab

## Lab Completed

- Broken 2FA logic

---

## Key Skills Practiced

- analyzing 2FA authentication flows  
- identifying logic flaws in multi-step authentication  
- automating large numbers of HTTP requests  
- bypassing rate limits and brute-force protections  

---

## Tooling Challenge

This lab required sending a large number of requests.

Limitations encountered:

- Burp Intruder (Community Edition) runs in a limited/demo mode  
- high-volume attacks are restricted without Burp Professional  

---

## Solution Approach

To overcome this limitation, I:

- installed the **Turbo Intruder extension**
- used a **Python script** to automate requests
- reduced the number of required requests from ~10,000 to ~2,000 using external insights

Without adapting my approach, the lab would not have been solvable using standard tools.

---

## Key Learning

This was an important lesson:

- tools have limitations  
- real-world pentesting often requires **custom solutions**  
- adapting your approach is more important than relying on tools alone  

---

# System Maintenance & Troubleshooting

Today I also updated my Kali Linux system:

```
sudo apt update && sudo apt upgrade
```

During the upgrade, I encountered:

- broken dependencies  
- package conflicts  
- incomplete upgrade state  

---

## Actions Taken

To resolve the issues, I:

- fixed broken packages  
- resolved dependency conflicts  
- handled dpkg-related errors  
- restarted the system  
- stabilized the environment without reinstalling  

---

## Key Learning

System troubleshooting is also part of being a pentester.

Skills developed:

- package management  
- dependency resolution  
- system recovery  
- maintaining a stable working environment  

---

# Practical Insight

Maintaining your own system is critical.

A pentester must be able to:

- fix their environment quickly  
- avoid downtime during engagements  
- troubleshoot issues independently  

---

# Progress Update

CWES Path Progress: Continuing steady progress

---

# Reflection

Today was a highly valuable day combining:

- API interaction  
- authentication bypass techniques  
- tool adaptation  
- system-level troubleshooting  

The most important lesson was understanding that:

> tools are not enough — problem-solving and adaptability are essential.

Successfully overcoming tool limitations and fixing system issues reinforced both **technical and practical skills** required in real-world penetration testing.