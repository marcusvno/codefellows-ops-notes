# Class 43 Reading Assignment

## Sniffing and Evasion 
- What is a Sniffing Attack in System Hacking? ([article](https://www.geeksforgeeks.org/what-is-sniffing-attack-in-system-hacking/))

## Questions
1. **Explain a Sniffing attack using non-technical terms.**
    - A sniffing attack is like someone peeking into your mail and packages as it's on the way from the post office to your house. 
2. **What are the two types of sniffing attacks and what are some pros and cons of each approach?**
    - Passive Sniffing: This type of sniffing involves monitoring and capturing data packets that are traveling through a network without altering them.
        - Pros: Harder to detect because it does not inject any traffic into the network.
        - Cons: Limited to what can be captured passively; may not capture encrypted data effectively.
    - Active Sniffing: Active sniffing involves injecting traffic into the network to either redirect or alter the communication for data interception.
        - Pros: Can discover more data by influencing network traffic, such as inducing responses from hosts.
        - Cons: Easier to detect due to the active injection of packets into the network and the potential disruption of normal network behavior.

3. **How does encryption protect traffic against sniffing attacks?**
    - Encryption makes it harder the attacker to be able to read the contents of packets and use those packets maliciously.