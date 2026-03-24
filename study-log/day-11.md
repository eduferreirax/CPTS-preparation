# CWES Preparation – Day 11

Date: March 22, 2026

## Study Time

CWES Preparation (HTB Academy): 2h 15m  
Web Practice (PortSwigger Labs): 54m  

Total Study Time: ~3h 09m

---

# Topics Covered

Today I focused on **web application security concepts related to access control and user role manipulation**, along with continued progress in the **CWES learning path**.

---

# HTB Academy Study (CWES Path)

## Module Progress

Today I completed **7 out of 8 sections** of the current module:

- Web Requests (Completed)

This module helped reinforce how HTTP requests work and how they can be manipulated during web exploitation.

---

## Key Concepts Studied

- structure of HTTP requests and responses  
- headers, parameters, and request bodies  
- how web applications process user input  
- how attackers manipulate requests to exploit vulnerabilities  

Understanding these fundamentals is essential for working effectively with tools like **Burp Suite**.

---

# Web Practice – PortSwigger Labs

Today I completed two labs focused on **access control vulnerabilities**.

---

## Labs Completed

- User role can be modified in user profile  
- User role controlled by request parameter  

---

## Key Skills Practiced

During these labs I worked on:

- intercepting and modifying requests using **Burp Suite**  
- analyzing application logic related to user roles  
- manipulating JSON request bodies  
- modifying cookies and parameters  
- testing access control mechanisms  

---

## Key Learnings

These labs demonstrated how improper access control can lead to **privilege escalation vulnerabilities**.

Important takeaways:

- user roles should never be controlled by client-side input  
- sensitive parameters must be validated server-side  
- cookies and request parameters can often be manipulated  
- access control flaws can lead to full administrative access  

---

## Performance Review

- One lab was solved **completely without using the solution**  
- The second lab required checking the solution for a small detail  

However, I was already on the **correct path**, which shows improvement in:

- understanding application logic  
- identifying attack vectors  
- reasoning through exploitation steps  

---

# Practical Insight

These labs reinforced a critical concept in web security:

> Applications should never trust user-controlled input for authorization decisions.

Even small implementation mistakes can allow attackers to:

- escalate privileges  
- access restricted areas (e.g., /admin)  
- perform unauthorized actions  

---

# Progress Update

CWES Path Progress: **7 / 8 sections completed (current module)**

---

# Reflection

Today was a strong day for developing **web exploitation skills**.

Key improvements:

- better understanding of access control vulnerabilities  
- improved ability to manipulate requests using Burp  
- increased confidence in solving labs without relying on solutions  

Even when I needed to check the solution, I was already very close to the correct approach.

This shows that my **reasoning process is improving**, which is essential for real-world pentesting and bug bounty hunting.

Consistency and continued practice in web labs will be key to mastering these concepts.