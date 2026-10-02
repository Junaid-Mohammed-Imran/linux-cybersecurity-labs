# Day 6 — Access Control

## Topics Covered

- Authorization Fundamentals
- Broken Access Control
- Horizontal Access Control
- Vertical Access Control
- IDOR
- Privilege Escalation
- Access-Control Testing

## Key Concepts

### Authorization

Authorization determines what an authenticated user is allowed to access or perform.

- Authentication → Who are you?
- Authorization → What are you allowed to do?

### Broken Access Control

Broken Access Control occurs when a user can access or perform something they are not authorized to access or perform.

Authorization should be enforced by the server.

### Horizontal Access Control

Controls access between users at the same privilege level.

Example:
A student accessing another student's private marks.

### Vertical Access Control

Controls access between different privilege levels.

Example:
A normal user accessing an admin-only function.

### IDOR

IDOR (Insecure Direct Object Reference) occurs when an application uses a direct reference to an object but fails to verify whether the current user is authorized to access it.

The problem is not the ID itself. The problem is missing authorization checks.

### Privilege Escalation

Privilege escalation occurs when a user gains access or permissions beyond what they should have.

- Vertical → gaining higher privileges
- Horizontal → accessing another user's resources

## Access-Control Testing

Important checks include:

- Identify different user roles.
- Identify what each role should access.
- Test access to other users' resources.
- Test higher-privileged functions.
- Verify that authorization is enforced on the server.
- Do not rely only on hidden buttons or frontend restrictions.

## Practical Lab

**Platform:** PortSwigger Web Security Academy

**Lab:** Unprotected admin functionality

**Difficulty:** Apprentice

**Status:** Solved ✅

### Practical Work

I tested the authorized PortSwigger lab and identified an unprotected administrator functionality.

The lab demonstrated how an application can expose administrative functionality without properly enforcing access control.

## What I Learned

I learned that authentication alone does not determine what a user can access.

I also learned the difference between horizontal and vertical access control, how IDOR relates to authorization failures, and why server-side authorization checks are important.

> All practical testing was performed only in the authorized PortSwigger Web Security Academy lab.
