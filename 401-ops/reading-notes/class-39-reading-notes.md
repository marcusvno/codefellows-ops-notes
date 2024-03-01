# Class 39 Reading Assignment

## SQLi with Burp Suite, WebGoat
- Understanding SQL Injection, Identification and Prevention ([link](https://www.varonis.com/blog/sql-injection-identification-and-prevention-part-1/))

## Questions

1. **What is SQL injection?**
    - SQL injection is the act of using SQL code in an input and accessing/breaking/manipulating the SQL database in the backend to gain access to data the user shouldn't. It is similar to XSS attacks but attack the database that powers the web application rather than vulnerabilities in the site's source code itself.
2. **Can you give an example of how a hacker could use SQL injection to gain unauthorized access?**
    - If the input isn't properly sanitized the hacker could use something like 'or 1=1' to trick the SQL to assume either the password *or* 1=1 has to be correct to gain access. 1=1 is always True, so it hacker bypasses the authentication process. 
3. **What are some ways to prevent SQL injection attacks on a web server?**
    - Sanitizing queries. Using frameworks like Rails or Django that automatically utilize best practices to deal with the most common of SQL injections. Web application firewalls can block most of the telltale signs of an injection attack. 
