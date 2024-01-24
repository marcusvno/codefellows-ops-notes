# Class 12 Reading Assignment

## Log Analysis with Splunk

What is a SOC? - ([link](https://www.splunk.com/en_us/data-insider/what-is-a-security-operations-center.html))

## Questions

1. **What are three tasks which SOCs often perform?**
    - The Security Operation Center, which consists of analysts and engineers, oversee all activity in servers, databases, networks, endpoint devices, applications, etc, so they can:
      - Pinpoint security threats and thwart them as quickly as possible.
      - Assess vulnerabilities and penetrations.
      - Monitor and gather threat intelligence on known risks.
      - Analyze the organization's security posture, ensuring that you're using security tools and other tech optimally and assessing what is and isn't working.
2. **Explain what a SIEM solution is and how the SOC utilizes it in non-technical terms.**
    - A Security Information and Event Management (SIEM) solution is an application that gathers and analyzes logs and data from multiple sources throughout a network. It gives SOC analysts the ability to comb through large amounts of indexed data and formats that data into a single unified format so that engineers don't have to hop between the differences of logging formats in Windows, Linux, etc. On top of this, some SIEM, like Splunk, have a robust querying language (similar to SQL) to allow extensive searching and filtering of the data. In non-technical terms, the SOC is the HQ where all security information is collects and analyzed for dealing with threats and incidents quickly.
3. **How does the typical SOC team structure resemble the structure of an IT Help Desk.**
    - Both SOC teams and IT Help Desk have a tiered system. Team members have different levels (SOC Analyst I, SOC Analyst II, etc) which have different levels of responsibilities and areas of expertise. Both are utilizing a structure similar to a chain of command in the military for easy division of labor, escalation, and team management.
