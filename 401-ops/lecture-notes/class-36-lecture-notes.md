# Class 36 - Web Applications

Web application are programs allowing better communication between businesses and their customers by way of a web browser interface.
- Frontend is usually created using languages like HTML, CSS, and JavaScript supported by major browser.
- Backend uses a programming stack
  - LAMP
  - MEAN
  - etc.
- Unlike mobile apps, there is no specific SDK for developing web applcations. 

## Web Application Security
- Careers in Application

## OWASP
- **Open Web Application Security Project (OWASP)** is an international non-profit organization dedicated to web application security, most known for it's list of top ten web application vulnerabilities.

- The **OWASP Top 10** is a regularly updated report outlining security concerns for web application security and the top 10 most critical risks
  - Extremely common in security interviews!

### OWASP TOP 10 (Nov 2021)
1. Broken Access Control
2. Cryptographic Failures
3. Injection
4. Insecure design
5. Security Misconfiguration
6. Vulnerable and Outdated components
7.- Identification and Authentication failures
8. Software and Data Integrity Failures
9. Security Loggig and Monitoring Falures
10. Server-Side Request Forgery (SSRF)

[!owasp-top-ten](https://owasp.org/www-project-top-ten/assets/images/mapping.png)

#### A01 Broken Access Control
#### A02 Cryptographic Failures
#### A03 Injection
#### A04 Insecure design
#### A05 Security Misconfiguration
#### A06 Vulnerable and Outdated components
#### A07 Identification and Authentication failures
#### A08 Software and Data Integrity Failures
#### A09 Security Loggig and Monitoring Falures
#### A10 Server-Side Request Forgery (SSRF)

## Cross-Site Scripting
- Reflect XSS
  - Malicious code is included in a URL (or other input) that is sent to a user  adn then reflected back to the user in response.
  - The attack then tries to convince the user