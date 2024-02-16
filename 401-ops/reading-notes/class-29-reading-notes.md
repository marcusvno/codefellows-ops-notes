# Class 29 Reading Assignment

## Modeling a Web Application

- Application Threat Modeling ([article](https://owasp.org/www-community/Application_Threat_Modeling))
- A Beginners Guide To The STRIDE Security Threat Model ([article](https://www.ockam.io/learn/blog/introduction_to_STRIDE_security_model))

## Questions

1. **Explain threat modeling using real-world non-technical examples.**
   - Threat modeling is about protecting your assets, and other valuables, from possible threats and dangers. For instance, a store has their inventory, their cash, their staff, and maybe a customer database. A threat model would consider the threats to each. Is the inventory prone to shoplifting? Is the point of sale secure? Is customer data backed up? Once you identify the various possible scenarios, you can start planning on shoring up those problems: antitheft personnel, secure point of sale systems, valueable merchandise held in secured locations or under the watchful eye of security cameras, etc. The final step is to always stay on top of the changing threat landscape and review regularly to see where the implementation if failing and where it is succeeding.
2. **What are the four questions that can help us organize threat modeling?**
   - What are we working on?
   - What can go wrong?
   - What are we going to do about it?
   - Did we do a good job?
3. **You are the project lead for a new application. How would you explain the benefits of Threat Modeling to the rest of the team?**
   - Threat modeling will inform how we build the application to ensure that we are secure from the start. Better to start off from a solid foundation than to develop a ton of tech debt and have to rewrite the entire codebase due to a zero day exploit or unforeseen vulnerability. While secure development may slow down starting speed, it pays immense dividends in not having to refactor or rewrite the code later, which can cost valuable time, money, and resources. Particularly if an active application has to be taken offline to patch the vulnerabilities.

## Additional Resources

- Threat Modeling Security Fundamentals ([article](https://docs.microsoft.com/en-us/learn/paths/tm-threat-modeling-fundamentals/))
