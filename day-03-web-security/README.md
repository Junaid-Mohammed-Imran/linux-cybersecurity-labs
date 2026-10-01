# Day 3 — Web Security Fundamentals

## Topics Covered

- Client and Server
- HTTP Requests and Responses
- HTTP Methods
- HTTP Status Codes
- Cookies and Sessions
- Authentication and Authorization
- Multi-Factor Authentication (MFA)
- OWASP and Web Vulnerabilities
- SQL Basics
- SQL Injection (SQLi)
- Cross-Site Scripting (XSS)

## Key Concepts

### Client and Server
- Client sends a request.
- Server processes the request and sends a response.

### HTTP
- GET → Retrieve data
- POST → Send data
- PUT → Update data
- DELETE → Remove data

### Common Status Codes
- 200 → OK
- 301 → Redirect
- 400 → Bad Request
- 401 → Unauthorized
- 403 → Forbidden
- 404 → Not Found
- 500 → Server Error

### Cookies and Sessions
Cookies are small pieces of data stored by a website in the browser.
Sessions help websites maintain a user's state, such as a login session.

Important cookie security attributes:
- Secure
- HttpOnly
- SameSite

### Authentication and Authorization
- Authentication → Who are you?
- Authorization → What are you allowed to do?
- MFA → Uses two or more authentication factors.

### Web Vulnerabilities
- Broken Access Control → A user can access something they should not.
- SQL Injection → User input changes an SQL query.
- XSS → Malicious JavaScript runs in another user's browser.

### SQL Basics
- SELECT → Retrieve data
- INSERT → Add data
- UPDATE → Change data
- DELETE → Remove data
- WHERE → Filter data

### SQL Injection Defense
Use parameterized queries / prepared statements.

### XSS Defense
Properly validate and encode user input/output.

## Practical — Browser DevTools

### Website
example.com

### Observation
The browser sent an HTTP GET request to the website.

Request Method:
GET

Request URL:
https://example.com/

Status Code observed:
304 Not Modified

The Response tab showed the HTML returned by the server.

### What I Learned

I learned how a browser communicates with a web server using HTTP requests and responses. I also learned basic web-security concepts including authentication, authorization, sessions, SQL Injection, XSS, and access control.

> Practical work was performed on example.com for educational observation only.
