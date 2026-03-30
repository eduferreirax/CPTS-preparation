# CWES Preparation – Day 17

## Study Time
- **CWES Path**: 00:51:54
- **Web Practice**: 00:39:32
- **Lab Practice**: 00:18:14
- **Python Practice**: 01:16:36
- **Total Study Time**: 03:06:16

# Topics Covered
Today's session marked the completion of the Back End Components module on HTB Academy. Practical efforts were heavily focused on unassisted execution of UNION-based SQL Injection attacks to extract sensitive data. Additionally, I dedicated significant time to advancing my Python scripting skills.

# HTB Academy Study (CWES Path)
## Module Progress
- Back End Components (Completed)
  - Development Frameworks & APIs (Completed)

## Key Concepts Studied
- Understanding the role of Development Frameworks and APIs in modern web application architecture.
- Consolidating knowledge on how backend servers, web servers, databases, and APIs interact.
- Identifying security implications and potential misconfigurations across different backend layers.

# Web Practice – PortSwigger Labs
## Labs Completed
- SQL injection UNION attack, finding a column containing text (Solved Unassisted)
- SQL injection UNION attack, retrieving data from other tables (Solved Unassisted)

## Key Skills Practiced
- Performing UNION-based SQL Injection (SQLi) attacks.
- Enumerating the number of columns returned by the original query.
- Probing individual columns to identify their supported data types (specifically targeting string/text compatibility).
- Extracting sensitive data (e.g., usernames and passwords) from arbitrary database tables.

## Key Learnings
- Successfully executing these attacks without relying on official solutions demonstrates a solidifying grasp of SQLi mechanics. 
- Ensuring the injected `UNION SELECT` payload perfectly matches the column count and data types of the original query is the most critical step in this attack vector.

# Lab Practice
- **Python Scripting (~1h 16m)**: Continued writing and refining custom scripts. Focused on implementing new concepts to improve logic flow, which will eventually aid in automating tedious enumeration tasks during web assessments.
- **General Lab Practice (~18m)**: Supplementary hands-on practice to reinforce the day's core concepts.

# Tools Used
- PortSwigger Labs
- Python
- Burp Suite

# Challenges Faced
- Manually determining the correct number of columns and finding the specific column that accepts string data types during the UNION attacks without external hints.

# How I Solved Them
- Relied on a strict, methodical enumeration process: injecting `ORDER BY` or `UNION SELECT NULL` incrementally until the application returned a normal response, then systematically substituting `NULL` with string values to identify target columns. 

# Progress Update
- **Milestone Reached**: 100% completion of the "Back End Components" module on HTB Academy.
- Achieved independence in solving intermediate-level UNION SQLi labs.

# Reflection
Completing the Back End Components module provides a highly necessary architectural perspective that makes identifying vulnerabilities much more intuitive. I am particularly proud of solving two complex UNION SQLi labs completely unassisted today. Relying on my own methodology rather than hints proves that the theoretical concepts are successfully translating into practical, real-world hacking skills. The continuous integration of Python scripting alongside these web labs is proving to be a highly effective routine.