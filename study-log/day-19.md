# CWES Preparation – Day 19

## Study Time
- **Lab Practice**: 01:29:04
- **Total Study Time**: 01:29:04

# Topics Covered
Today was a strategically shorter session focused on maintaining consistency while prioritizing rest for better cognitive performance. Despite the reduced hours, I made solid progress on a target machine, covering Supabase infrastructure reconnaissance, Server-Side Request Forgery (SSRF) filter bypasses, and Privilege Escalation vectors involving C and Rust[cite: 1].

# Lab Practice
## Labs Completed
- Target Practice Machine (In Progress)

## Key Skills Practiced
- Enumerating Supabase infrastructure by targeting default ports such as 54321 for the REST API and 54323 for the Dashboard[cite: 1].
- Discovering database tables via the Schema Visualizer and querying them through the `/rest/v1/[table_name]` API endpoint[cite: 1].
- Bypassing basic SSRF string filters that block `127.0.0.1` or `localhost` by converting the loopback address into its decimal IP format, `2130706433`[cite: 1].
- Crafting malicious `.so` shared objects in C to exploit applications that dynamically load libraries using `dlopen()` and `dlsym()`, achieving Remote Code Execution (RCE)[cite: 1].
- Abusing `sudo` privileges on Rust's `cargo` package manager by creating a new project and modifying `main.rs` to alter system binary permissions (like `/bin/bash`) for Privilege Escalation[cite: 1].

## Key Learnings
- If PostgreSQL Row Level Security (RLS) is disabled in a Supabase environment, the REST API can be exploited to dump the entire contents of a table without requiring high-level privileges[cite: 1].
- Once an SSRF vulnerability is confirmed, internal API management endpoints (such as `/api/search` or `/api/dashboards`) become prime targets for extracting cleartext credentials or secrets[cite: 1].
- Write access to a plugin directory in C applications is a critical vulnerability if the attacker can compile and upload a shared object with an initialization function (e.g., `plugin_init`)[cite: 1].

# Tools Used
- API Clients / Browser DevTools
- C Compiler (for `.so` payload generation)
- Rust / Cargo

# Challenges Faced
- Managing fatigue and ensuring I have the necessary focus to successfully compromise a complex target machine.

# How I Solved Them
- I made the professional decision to pause the exploitation phase, recognizing that resting now will yield better performance. I have set a strict goal to return tomorrow with a fresh mindset to conquer the machine and hit a 5-hour study target.

# Progress Update
- Initial enumeration and foothold strategies on the target machine are documented and in progress. 

# Reflection
Consistency in cybersecurity training doesn't always mean pushing to the point of burnout. Recognizing fatigue and strategically stepping away is essential for long-term success. Even in this brief 1.5-hour window, I managed to deeply analyze critical modern vulnerabilities like Supabase RLS misconfigurations and SSRF decimal bypasses. The foundation is set to crush the machine tomorrow.