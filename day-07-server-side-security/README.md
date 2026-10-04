Day 7 — Server-Side Security

Topics Covered

Topic 1 — SSRF

- Learned what Server-Side Request Forgery (SSRF) is.
- Understood how an attacker can make a server send requests to unintended locations.
- Learned the difference between external and internal SSRF.
- Internal SSRF can allow access to resources that are normally inaccessible to the attacker.

Topic 2 — Command Injection

- Learned what Command Injection is.
- Understood how malicious input can cause an application to execute unintended operating system commands.
- Compared Command Injection with SQL Injection.

Topic 3 — Path Traversal

- Learned how Path Traversal can allow access to files outside the intended directory.
- Understood the purpose of "../" in paths.
- Learned that the vulnerability occurs when an application fails to properly restrict file paths.

Topic 4 — File Upload Vulnerabilities

- Learned how insecure file-upload functionality can create security risks.
- Understood the importance of validating file type, extension, content, size, storage location, and execution permissions.

Topic 5 — Server-Side Vulnerability Testing

- Learned how to identify user-controlled input.
- Followed where the input goes on the server.
- Identified what server-side operation the input influences.
- Learned to test whether proper security controls are applied.

Practical Lab

Platform: PortSwigger Web Security Academy

Lab: Basic SSRF against the local server

What I Did

- Intercepted the stock-check request using Burp Suite.
- Sent the request to Burp Repeater.
- Modified the "stockApi" parameter to access the internal "/admin" endpoint.
- Identified the administrator functionality.
- Used the SSRF vulnerability to access the internal delete functionality.
- Successfully completed the lab.

Tools Used

- Burp Suite
- PortSwigger Web Security Academy

Key Learning

«SSRF occurs when a vulnerable server can be manipulated into making requests to resources that the attacker should not be able to access directly.»

Status

✅ Theory Completed
✅ Practical Lab Completed
