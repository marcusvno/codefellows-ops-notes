# Class 37 Reading Assignment

## Automated AppSec with ZAP
- Getting Started with ZAP  ([article](https://www.zaproxy.org/getting-started/))

## Questions

1. **What are the three common stages of the Penetration Testing process and what tasks are performed at each one?**
    - **Explore -** The tester attempts to learn about the system being tested. This includes trying to determine what software is in use, what endpoints exist, what patches are installed, etc. It also includes searching the site for hidden content, known vulnerabilities, and other indications of weakness. 
    = **Attack -** The tester attempts to exploit the known or suspected vulnerabilities to prove they exist.
    - **Report -** The tester reports back the results of their testing, including vulnerabilities, how they exploited them and how difficult the exploits were, and the severity of exploitation.
2. **Explain a “man-in-the-middle proxy” in non-technical terms.**
    - A man in the middle proxy stands between the tester's browser and web application. Think of it a like trying to pass notes to someone in class but there is a person in the middle who relays the messages, but they can also inspect the notes and change things if needed.
3. **What are the 2 spiders available for use in ZAP?**
    - ZAP offers two types of spiders: the traditional ZAP spider and the AJAX spider.
4. **What situations are they best suited for?**
    - A traditional spider is fast and good for basic websites. AJAX spider is beter for modern web apps that use a lot of JavaScript as it simulates a real user by invoking browsers. 


## Additional Resources
- Python Tools for Hackers ([article](https://hackersonlineclub.com/python-tools/))