# Class 03 - Cyber Risk Analysis

## Overview

- **Risk**
  - The _likelihood_ and _impact_ of a threat actor exploiting a vulnerability.
- **Vulnerability**
  - A weakness that could be triggered accidentally or exploited intentionally to cause a security breach.
- **Threat**
  - The potential for someone or something to exploit a vulnerability, whether intentional or unintentional.

Risk can vary depending on the business or organization under threat. The pentagon and a small business may both be vulnerable to the same exploit but that does not mean their risk or threat is **_equal_**.

## Security and Risk Management

- **What is the risk management lifecycle?**
  - _Categorize, Classify, and Value Assets_
    - Identify what could be threatened and the value of those assets if threatened. This will be used as part of the equation to determine whether the losses and impact of a risk incident occuring is worth mitigating, preventing, or accepting. Everything has a bottom line value.
  - _Know/Identify Threats and Vulnerabilities_
    - Identifying what the risks are: threat actors and vulnerabilities. What and where the risk might be coming from. Nothing is a fully closed system and therefore risk is never fully removed. New vulnerabilities are found, people can be phished, coerced, or blackmailed, etc.

<center><img src="https://codefellows.github.io/ops-401-cybersecurity-guide/curriculum/class-03/slides/assets/03_02.png"/></center>

- **Risk Analysis**
  - _Qualitative Analysis_ is subjective in nature and uses words like “high,” “medium,” “low” to describe the likelihood and severity of the impact of a threat exposing a vulnerability.
  - _Quantitative Analysis_ is objective and numbers-driven.
    - Uses numerical data and mathematical models to assess and quantify risks
    - Assigns monetary values to risk components.
    - Allows for cost-benefit analysis, return on investment calculations, and prioritization of risk mitigation efforts

<center><img src="https://codefellows.github.io/ops-401-cybersecurity-guide/curriculum/class-03/slides/assets/03_03.png" width=500/></center>

- **Risk Response and Mitigation**

  - Reduce
  - Avoid
  - Transfer
  - Accept/Reject

- **Monitor and Report**
  - Now that we've implemented a mitigation response we have to monitor to see if that response is operating at acceptable levels.
    - Did the reduction/avoidance/tranferance of risk actually diminish the number of incidents we're seeing and the impact on our orgnization?
    - If we accepted the risk, is the impact still within the thresholds of our acceptance levels? Say Walmart is willing to write off $100k in annual inventory losses to shoplifting, are we still under that number? Etc.

## Quantitative Analysis Breakdown

### Single Loss Expectancy Formula

- **Asset Value (AV)**: How come is the asset worth?
- **Exposure Factor (EF)**: What percentage of Asset Value is lost?
- **Single Loss Expectancy (SLE)**: What does it cost if it happens once?

The formula is: `SLE = AV x EF`

```
Single Loss Expentancy = Asset Value x Exposure Factor
```

Basically: What is the value of the asset times the chances of the asset being lost equals the cost if the asset is lost one time.

### Annual Loss Expectancy Formula

- **Annual Rate of Occurence (ARO)**: How often will this happen per year?
- **Annualized Loss Expentancy (ALE)**: What would it cost per year if we do nothing?

The formula is: `ALE = SLE x ARO`

```
Annualized Loss Expentancy = Single Loss Expentancy x Annual Rate of Occurence
```

Basically: How much does it cost if it happens once times the chances of it happening per year equals the annual cost of if we do nothing for the entire year.

**Total Cost of Ownership (TCO)**: The TCO is the mitigation cost: upfront cost + ongoing cost.

### Example Quantative Risk Exercise

- Laptop - Theft/Loss (unencrypted)
  - Laptop ($1000) + PII (Personal Identifiable Information) ($9000) per loss (**A**sset **V**alue)
  - It a 100% loss. (**E**xposure **F**actor)

The formula: `SLE = AV x EF`

- Loss per laptop is $10,000 (AV) x 100% (EF) = $10,000 (SLE)

- The organization loses 25 laptops per year (ARO)
  `ALE = SLE x ARO`
  - $10,000 (SLE) x 25 (ARO) = **$250,000** Annualized Loss Expentancy

## Qualitative Analysis

Qualitative Analysis is a softer approach and does not use data quantification.

- Rating system is used instead.
- Requires judgement based on best practices, intuition, and experience.

Methods can include:

- Brainstorming
- Delphi Technique ([article](https://www.rand.org/topics/delphi-method.html))
- Questionnaires
- Storyboarding
- Focus Groups
- Surveys
- Checklists
- One on one meetings
- Interviews

## Risk Management Options

- **Risk Acceptance**: Acknowledge the risk exists but do nothing.
- **Risk Ignore**: You ignore the risk exists.
- **Risk Avoidance**: Avoid the risky behaviour.
- **Risk Mitigation**: Reduce the risk.
- **Risk Transference**: Moving the risk to a third party for coverage. (Think car insurance)

### Example: Windows Vista Server
- **Risk Acceptance**: Acknowledge the risk exists but do nothing.
- **Risk Avoidance**: Update it to Windows 10.
- **Risk Mitigation**: Reduce the usage of the Windows Vista Server.
- **Risk Transference**: Cybersec insurance?

## NIST ([link](https://www.nist.gov/cyberframework))

- **Can risk be eliminated?**
  - Cyber Risk can't be fully eliminated, but it can be significantly mitigated.
  - Residual risk consists of the risk remaining after security controls have been put in place as a means of risk mitigation.

The **NIST Risk Management Framework** (RMF) is a voluntary guidance, based on existing standards, guidelines, and practices for organizations to better manage and reduce cybersecurity risk. 

## Cyber Hygiene

- **What is cyber hygiene?**
  - Cyber hygiene includes practices and precautions that faciliate keeping senstitive data organized, safe, and secure from exfiltration and attack.

- **How do security teams work mitigate risk for their employer or clientele?**
  - Regulary evaluate for cyber hygiene
  - Perform vulnerability scans and assessment
  - Generate risk assessments which faciliate better organizational decision making