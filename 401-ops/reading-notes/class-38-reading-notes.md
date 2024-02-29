# Class 38 Reading Assignment

## Attacking Juice Shop with Burp Suite 
- What is Burp Suite? ([article](https://www.technipages.com/what-is-burp-suite))

## Questions
1. **Explain how Burp Suite allows us to analyze web application traffic.**
    - Like Zed Attack Proxy (ZAP), Burp also uses a man-in-the-middle-proxy to analyze web application traffic and intercept requests and responses, allowing real-time reading and editing before they reach their destinations. 
2. **What does the Repeater tool allow us to do with requests?** 
    - Repeater allows you to import a web request and then make manual modifications to it and see the response side by side allowing you to make minor adjustments to attempted exploits and easily see if it’s working.
3. **Why might this be a useful tool for an attacker?**
    - Burp Suite offers valuable tools for attackers by enabling the interception and modification of web application traffic. This capability allows them to test applications for vulnerabilities by altering and observing the effects of different requests in real-time and helps with identifying potential security weaknesses to exploit.