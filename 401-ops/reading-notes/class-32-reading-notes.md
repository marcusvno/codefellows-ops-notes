# Class 32 Reading Assignment

## Malware Traffic Analysis with Wireshark 
- What Is Malware Analysis? Definition, Types, Stages, and Best Practices ([article](https://www.spiceworks.com/it-security/data-security/articles/what-is-malware-analysis-definition-types-stages-best-practices/))

## Questions
1. **You just started a new job as a Malware Analyst. Explain your job responsibilities to a family member.**
    - I'm the digital biologist, dissecting dangerous predators in hopes to understand how to stop them before they do any harm.
2. **What are the six steps of the Malware Analysis process? What’s a good mnemonic you can use to remember it?**
    1. Capture the malware.
      - Find malware to analysis. Or use a tool like HoneyDB to attract and capture some.
    2. Build a malware lab.
      - A sandboxed environment (usually made with VMS) to safely test and observe the malware.
    3. Install tools
      - Acquire and install the tools you'll need to analyze the malware.
    4. Record the baseline.
      - Before running the malware, take an assessment of how the environment operates prior to the malware affects it and document it
    5. Commence Investigation
      - Several phases of investigations can be performed in this step. (Not elaborated on in article)
    6. Document Results.
    - Cats Bake Iced Rodent Cakes Daily
3. **You are tasked with analyzing a new malware sample. Which type of malware analysis would you conduct first and why?**
    - Statis study to try and establish an indicator of compromise and the ware's nature and then a dynamic study to determine how the malware behaves. This behavioral study can try to further narrow down the facets of the malware's identity and traits.

![malware types](https://images.spiceworks.com/wp-content/uploads/2020/11/19071537/Malware-analysis.png)