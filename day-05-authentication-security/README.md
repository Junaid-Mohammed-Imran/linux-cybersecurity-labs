# Day 5 — Authentication Security

## Topics Covered

- Authentication Fundamentals
- Authentication Vulnerabilities
- Brute Force
- Credential Stuffing
- Username Enumeration
- Rate Limiting
- Password Hashing and Salting
- Session Security
- Multi-Factor Authentication (MFA)

## Key Concepts

### Authentication
Authentication verifies the identity of a user.

### Authentication vs Authorization
- Authentication → Who are you?
- Authorization → What are you allowed to do?

### Authentication Vulnerabilities
- Weak passwords
- Brute-force attacks
- Credential stuffing
- Username enumeration
- Missing rate limiting

### Password Security
- Passwords should not be stored in plaintext.
- Passwords should be securely hashed.
- Unique salts help protect against precomputed attacks.
- Dedicated password-hashing algorithms such as Argon2, bcrypt, or scrypt are commonly used.

### Session Security
- Sessions keep users logged in after authentication.
- Session IDs should be protected.
- Secure cookie attributes include:
  - Secure
  - HttpOnly
  - SameSite
- Session IDs should be regenerated after login.

### MFA
MFA uses two or more different authentication factors:
- Something you know → Password/PIN
- Something you have → Phone/Security key
- Something you are → Fingerprint/Face

## Practical Lab

**Platform:** PortSwigger Web Security Academy

**Lab:** Username enumeration via different responses

**Difficulty:** Apprentice

**Status:** Solved ✅

### Practical Work

- Captured the login request using Burp Suite.
- Used Burp Intruder with a Sniper attack.
- Tested the provided candidate usernames.
- Identified a username with a different response length.
- Confirmed the valid username through the login response.
- Practiced the authentication vulnerability in the authorized PortSwigger lab environment.

## What I Learned

I learned how authentication vulnerabilities can reveal valid usernames and how weak authentication mechanisms can be tested in a controlled environment.

I also practiced using Burp Suite Intruder to automate testing of the provided candidate usernames.

> All practical testing was performed only
