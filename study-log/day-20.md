# CWES Preparation – Day 20

## Study Time
- **Bug Bounty**: 04:44:56
- **Lab Practice**: 00:36:45
- **Total Study Time**: 05:21:41

# Topics Covered
Today's session marked a major transition from structured labs to real-world target exploitation. I dedicated significant time to Bug Bounty hunting, applying a newly developed, comprehensive methodology named "SuperHunterV5". Additionally, I tackled a target machine on HackingClub, focusing heavily on Supabase infrastructure reconnaissance, Server-Side Request Forgery (SSRF) bypasses, and advanced Privilege Escalation techniques using C and Rust.

# Bug Bounty Practice
## Methodology Development
- Designed and documented a complete, modern Bug Bounty methodology titled **SuperHunterV5**, utilizing AI (Claude) to structure the reconnaissance, exploitation, and reporting workflows. 

## Live Targets
- Transitioned to practicing on live targets, actively testing the SuperHunterV5 methodology to identify real-world vulnerabilities and improve practical hunting efficiency.

# Lab Practice
## Labs Completed
- HackingClub Machine

## Key Skills Practiced & Learnings
- [cite_start]**Supabase Reconnaissance**: Conducted infrastructure reconnaissance on Supabase environments, targeting default ports 54321 (REST API/PostgREST) and 54323 (Dashboard/Studio)[cite: 1].
- [cite_start]**API Enumeration**: Discovered table names via the Schema Visualizer and directory brute-forcing on the API[cite: 3]. [cite_start]Interacted with the database using the standard `/rest/v1/[table_name]` API endpoint[cite: 2].
- [cite_start]**Row Level Security (RLS) Exploitation**: Analyzed RLS configurations, a PostgreSQL feature that filters row access based on defined policies[cite: 4]. [cite_start]Exploited disabled RLS policies to execute a full data dump via the REST API without requiring high-privilege tokens[cite: 5]. [cite_start]Identified that missing RLS is a critical vulnerability, often rated P1/P2 in Bug Bounty programs[cite: 6].
- [cite_start]**SSRF & Filter Bypasses**: Executed Server-Side Request Forgery (SSRF) to force the server to access internal endpoints, such as a local Grafana instance on port 3000[cite: 7]. [cite_start]Bypassed basic SSRF string filters for `127.0.0.1` or `localhost` by converting the IP to its decimal representation (`2130706433`)[cite: 8]. [cite_start]Leveraged the SSRF to hit internal management endpoints (e.g., `/api/search`, `/api/dashboards`) to extract cleartext credentials and secrets[cite: 9].
- [cite_start]**Privilege Escalation (C)**: Investigated binary exploitation vectors in C applications utilizing `dlopen()` and `dlsym()` for dynamic library loading[cite: 10]. [cite_start]Achieved Remote Code Execution (RCE) by compiling a malicious `.so` shared object with an initialization function (`plugin_init`) and writing it to a vulnerable plugin directory[cite: 11].
- [cite_start]**Privilege Escalation (Rust)**: Escalated privileges using Rust's `cargo` package manager by abusing assigned `sudo` permissions[cite: 12]. [cite_start]Created a new project using `cargo new` and manipulated the `main.rs` file to alter system binary permissions (e.g., `/bin/bash`) to secure root access[cite: 13].

# Tools Used
- Bug Bounty Platforms (Live Targets)
- Claude (Methodology Structuring)
- HackingClub Platform
- API Clients (Postman/Burp Suite)
- C Compiler (`gcc`) & Rust (`cargo`)

# Challenges Faced
- Structuring a massive, comprehensive Bug Bounty methodology from scratch that covers everything from initial recon to complex exploitation without becoming overwhelming.
- Bypassing strict SSRF filters and understanding the interaction between custom `.so` libraries and C application logic.

# How I Solved Them
- Leveraged AI to organize and streamline my thought process, resulting in the highly structured "SuperHunterV5" methodology.
- Applied IP obfuscation techniques (decimal IPs) for the SSRF and studied the mechanics of `dlopen()` to properly construct the malicious shared object for privilege escalation.

# Progress Update
- Shifted focus toward live Bug Bounty targets, executing over 4.5 hours of active hunting using a custom, newly refined methodology.

# Reflection
Today was a massive leap forward. Moving from purely academic labs to real-world Bug Bounty hunting with a structured methodology (SuperHunterV5) fundamentally changes how I approach targets. The HackingClub machine provided excellent, high-level technical exposure—specifically the intricacies of Supabase misconfigurations (RLS) and advanced SSRF filter bypasses. Combining these modern web vulnerabilities with low-level privilege escalation techniques (C/Rust) is building exactly the kind of holistic offensive mindset required for the CWES and professional penetration testing.