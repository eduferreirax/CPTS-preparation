# CPTS Preparation – Day 07

Date: March 18, 2026

## Study Time

Web Practice (PortSwigger Labs): ~5h 28m  

Total Study Time: ~5h 28m

---

# Topics Covered

Today I introduced **PortSwigger Web Security Academy labs** into my study routine.

The entire focus of the day was on **JWT (JSON Web Token) attacks**, using Burp Suite extensively.

This was my first deep exposure to **web exploitation at a more realistic level**, and it was significantly more challenging than previous labs.

---

# Web Practice – PortSwigger Labs

Today I completed multiple labs related to **JWT authentication bypass techniques**.

All labs were solved using **Burp Suite**, which I used throughout the entire session.

---

## Labs Completed

- JWT authentication bypass via unverified signature  
- JWT authentication bypass via flawed signature verification  
- JWT authentication bypass via weak signing key  
- JWT authentication bypass via jku header injection  
- JWT authentication bypass via jwk header injection  
- JWT authentication bypass via kid header path traversal  

---

# Key Skills Practiced

During these labs I practiced:

- intercepting and modifying HTTP requests using **Burp Suite**
- analyzing JWT structure (header, payload, signature)
- manipulating JWT tokens to bypass authentication
- exploiting weak or misconfigured signature validation
- understanding how servers fetch keys dynamically (jku / jwk)
- exploiting path traversal through JWT headers (kid)
- debugging JSON formatting issues during exploitation

---

# Key Learning Moment

One of the most impactful moments today was during the lab:

**JWT authentication bypass via jku header injection**

I spent nearly **2 hours troubleshooting the exploit**, which ultimately failed due to a **small JSON formatting issue (a missing or misplaced comma)**.

This reinforced an important lesson:

- exploitation often fails due to **minor syntax or formatting issues**
- attention to detail is critical in web exploitation
- debugging is a core skill in real-world pentesting

---

# Tools Used

- **Burp Suite** (used throughout all labs)
- browser developer tools
- JWT analysis and manipulation techniques

Total Burp usage today: ~5h+

---

# Transition to Web Hacking

Today marked a significant shift toward **web application security**.

Compared to previous machines, these labs required:

- more precision
- deeper understanding of HTTP and authentication flows
- manual testing and debugging

This felt like a **"baptism by fire" into web hacking**.

---

# Next Steps

Tomorrow I plan to:

- continue JWT-related labs on **PentesterLab**
- reinforce the same concepts in a different environment
- start building consistency in web exploitation techniques

---

# Reflection

Today was one of the most challenging and important study days so far.

Focusing entirely on **JWT attacks** helped me understand:

- how authentication mechanisms can fail
- how small misconfigurations can lead to full account takeover
- how important precision and debugging are in web security

Spending over 5 hours using **Burp Suite** also helped me become more comfortable with:

- intercepting requests
- modifying payloads
- analyzing server responses

This was a major step toward becoming proficient in **web penetration testing and bug bounty hunting**.