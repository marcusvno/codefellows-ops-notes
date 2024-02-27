# Class 36 Reading Assignment

## XSS with w3af, DVWA
- Cross Site Scripting ([link]())

## Questions
1. **Explain how a cross-site scripting attack works in non-technical terms.**
    - Cross site scripting allows attackers to alter, forge, or manipulate the interactions users have with a web application. If a user has admin access, this may allow an attacker to masquerade as them and gain full control over the web site/application.
2. **What are the three types of XSS attacks?**
    - **[Reflected XSS](https://portswigger.net/web-security/cross-site-scripting#reflected-cross-site-scripting)**, where malicious scripts comes from the current HTTP request
    - **[Stored XSS](https://portswigger.net/web-security/cross-site-scripting#stored-cross-site-scripting)**, where the malicious script comes from the website's database.
    - **[DOM-based XSS](https://portswigger.net/web-security/cross-site-scripting#dom-based-cross-site-scripting)**, where the vulnerability exists in client-side code rather than server-side code.
3. **If an attacker successfully exploits a XSS vulnerability, what malicious actions would they be able to perform?**
    - Impersonate or masquerade as the victim user.
    - Carry out any action that the user is able to perform.
    - Read any data that the user is able to access.
    - Capture the user's login credentials.
    - Perform virtual defacement of the web site.
    - Inject trojan functionality into the web site.
4. **What are some security controls that can be implemented to prevent XSS attacks?**
    - **Filter input on arrival.** At the point where user input is received, filter as strictly as possible based on what is expected or valid input.
    - **Encode data on output.** At the point where user-controllable data is output in HTTP responses, encode the output to prevent it from being interpreted as active content. Depending on the output context, this might require applying combinations of HTML, URL, JavaScript, and CSS encoding.
    - **Use appropriate response headers.** To prevent XSS in HTTP responses that aren't inteded to contain any HTML or JavaScript, you can use the `Content-Type` and `X-Content-Type-Options` headers to ensure that browsers interpret the responses in the way you intend.
    - **Content Security Policy.** As a last line of defense you can use Content Security Policy (CSP) to reduce the severity the of any XSS that still occur.


## Additional Resources

- Security Report for In-Production Web Applications ([pdf](https://www.rapid7.com/globalassets/_pdfs/whitepaperguide/rapid7-tcell-application-security-report.pdf))

