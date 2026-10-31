# INTERNATIONAL CYBERSECURITY AND DIGITAL FORENSICS ACADEMY

## GRC103: Risk Assessment and Management Techniques

### Week 2 Practical Laboratory:
# Advanced Cybersecurity Risk Quantification and Control Investment Analysis

**Full Name:** Venesha Adhiambo Ochieng  
**Registration Number:** C11/26/CGRCE/17566  
**Email Address:** c11.cgrce2617566@icdfa.edu.ng  
**Cohort / Batch:** Cohort11  
**Date Submitted:** 31st October 2026

---

# Lab 3b: Advanced Cybersecurity Risk Quantification

## 1. Introduction

Welcome to the Cybersecurity Risk Quantification Lab. As a GRC professional, you must translate technical vulnerabilities into business impact. This lab will challenge you to perform end-to-end risk analysis for a critical business system.

## 2. Scenario

You are the lead GRC analyst at "SecureBank Financial." The CISO has provided you with data from a recent penetration test and vulnerability assessment of your new mobile banking platform. Your task is to quantify the financial risk, evaluate control options, and prepare an executive briefing.

## 3. Learning Objectives

- Calculate risk exposure using quantitative methods
- Perform cost-benefit analysis for security controls
- Create data-driven recommendations
- Develop executive-level risk reporting with visualizations

## 4. Dataset: Mobile Banking Platform Assessment

### System Context:

- Platform: "SecureMobile" banking application
- User Base: 500,000 active customers
- Average Transaction: $2,500
- Daily Transactions: 50,000

### Vulnerability Assessment Results:

#### Critical Finding 1: API Authentication Bypass

- Exploit Probability: 15%
- Systems Affected: Transaction processing system
- Potential Impact: Unauthorized fund transfers
- Maximum Single Incident Loss: $5,000,000
- Estimated Detection: 48 hours

#### Critical Finding 2: Database Injection Vulnerability

- Exploit Probability: 25%
- Systems Affected: Customer database
- Potential Impact: Data breach (PII + financial data)
- Records at Risk: 500,000 customer profiles
- Cost per Record: $250 (regulatory + notification)

#### Critical Finding 3: Session Hijacking

- Exploit Probability: 40%
- Systems Affected: User sessions
- Potential Impact: Account takeover
- Accounts at Risk: 5,000 simultaneous sessions
- Average Loss per Account: $1,500

### Control Options:

#### 1. Advanced API Security Gateway

- Cost: $350,000
- Effectiveness: 90% reduction in API vulnerabilities
- Maintenance: $50,000/year

#### 2. Web Application Firewall (WAF)

- Cost: $150,000
- Effectiveness: 75% reduction in web vulnerabilities
- Maintenance: $25,000/year

#### 3. Multi-Factor Authentication Enhancement

- Cost: $200,000
- Effectiveness: 95% reduction in account takeover
- Maintenance: $30,000/year

# Phase 1: Risk Exposure Calculation

## Task 1: Calculate Annualized Loss Expectancy (ALE)

For each vulnerability, calculate:

### Single Loss Expectancy (SLE)

SLE = Asset Exposure x Loss per Unit

### Annual Rate of Occurrence (ARO)

ARO = Expected Number of Incidents per Year

### Annualized Loss Expectancy (ALE)

ALE = SLE x ARO

## Task 1.1 Critical Finding 1: API Authentication Bypass

**SLE** = $5,000,000

**ARO** = 15/100 = 0.15

**ALE** = $5,000,000 x 0.15 = $750,000

## Task 1.2 Critical Finding 2: Database Injection Vulnerability

**SLE** = Records at Risk x Cost per Record

= 500,000 x $250

= $125,000,000

**ARO** = 25/100 = 0.25

**ALE** = $125,000,000 x 0.25

= $31,250,000

## Task 1.3 Critical Finding 3: Session Hijacking

**SLE** = Accounts at Risk x Average Loss per Account

= 5,000 x $1,500

= $7,500,000

**ARO** = 40/100 = 0.40

**ALE** = $7,500,000 x 0.40

= $3,000,000

### Consolidated Risk Exposure Calculations

| Vulnerability | SLE (USD) | ARO | ALE (USD) |
|--------------|-----------|------|-----------|
| API Authentication Bypass | $5,000,000 | 0.15 | $750,000 |
| Database Injection | $125,000,000 | 0.25 | $31,250,000 |
| Session Hijacking | $7,500,000 | 0.40 | $3,000,000 |
| Total | $137,500,000 | - | $35,000,000 |

## Task 2: Prioritize Risks

Create a risk matrix showing:

- Vulnerability
- SLE
- ARO
- ALE
- Risk Priority Level

### Task 2.1 Risk Prioritization Matrix
| Vulnerability | SLE (USD) | ARO | ALE (USD) | Risk Priority Level |
|--------------|-----------|------|-----------|--------------------|
| Database Injection Vulnerability | $125,000,000 | 0.25 (25%) | $31,250,000 | Critical |
| Session Hijacking | $7,500,000 | 0.40 (40%) | $3,000,000 | High |
| API Authentication Bypass | $5,000,000 | 0.15 (15%) | $750,000 | Medium |
| Total | $137,500,000 | - | $35,000,000 | - |

## Task 2.2 Risk Prioritization Analysis

### Priority 1: Database Injection Vulnerability - Critical Risk

Database injection presents the highest financial exposure, with an ALE of $31,250,000, representing approximately 89.29% of the total estimated annual risk exposure. Successful exploitation could compromise up to 500,000 customer records containing personally identifiable information and financial data. Due to its substantial potential financial, regulatory, and reputational consequences, this vulnerability requires immediate executive attention and urgent remediation.

### Priority 2: Session Hijacking - High Risk

Session hijacking has an ALE of $3,000,000, accounting for approximately 8.57% of total annual risk exposure. With an assumed annual occurrence probability of 40%, it has the highest likelihood among the identified vulnerabilities. Successful exploitation could result in unauthorized account access, fraudulent transactions, and customer financial losses. This vulnerability requires high-priority remediation, particularly through stronger session management and enhanced multi-factor authentication.

### Priority 3: API Authentication Bypass - Medium Risk

API authentication bypass has an ALE of $750,000, representing approximately 2.14% of the total estimated annual financial exposure. Although it has the lowest modeled ALE, the vulnerability remains significant because it affects SecureBank Financial's transaction processing system and could facilitate unauthorized fund transfers. Remediation should focus on strengthening API authentication, authorization controls, transaction monitoring, and fraud detection.

Its Medium classification reflects the illustrative ALE thresholds, not necessarily its operational severity. Given the direct exposure of financial transactions, management may assign a higher treatment priority based on risk appetite and regulatory requirements.

---

## Task 3: Create Risk Visualization

### Task 3.1 Generate a Bar Chart Comparing ALE for All Vulnerabilities
## Task 3: Create Risk Visualization

### Task 3.1 Generate a Bar Chart Comparing ALE for All Vulnerabilities

 ![Task 3.1 - ALE Comparison](task%203.1.png)

### Task 3.2 Create a Pie Chart Showing Risk Distribution

 ![Task 3.2 - Risk Distribution](task%203.2.png)

### Task 3.3 Develop a Risk Heat Map (High/Medium/Low) Based on Probability and Impact

 ![Task 3.3 - Risk Heat Map](task%203.3.png)

# Phase 2: Control Evaluation

## Task 4: Cost-Benefit Analysis

For each control option, calculate:

- Initial Investment
- Annual Maintenance
- Risk Reduction (in $)
- Return on Investment (ROI)
- Payback Period

### Formulas used:

**Risk Reduction** = Current ALE x Control Effectiveness

**ROI** = ((Risk Reduction - Total Cost)/Total Cost)) x 100

**Payback Period** = ((Total Cost/Annual Risk Reduction)) x 12

Where:

Total Cost = Initial Investment + Annual Maintenance

---

## Task 4.1 Advanced API Security Gateway

**Initial Investment**

= $350,000

**Annual Maintenance**

= $50,000 per year

**Risk Reduction (in $)**

Current ALE = $750,000

Control Effectiveness = 90%

= $750,000 × 0.90

Risk Reduction = $675,000

**Return on Investment (ROI)**

First-Year Total Cost:

= $350,000 + $50,000 = $400,000

ROI = (($675,000 - $400,000)/$400,000) × 100

ROI = 68.75%

**Payback Period**

= ($400,000/$675,000) x 12

Payback Period = 7.11 months

---

## Task 4.2 Web Application Firewall (WAF)

**Initial Investment**

= $150,000

**Annual Maintenance**

= $25,000 per year

**Risk Reduction (in $)**

Current ALE = $31,250,000

Control Effectiveness = 75%

= $31,250,000 x 0.75

Risk Reduction = $23,437,500

**Return on Investment (ROI)**

First-Year Total Cost:

= $150,000 + $25,000 = $175,000

ROI = (($23,437,500 - $175,000)/$175,000) x 100

ROI = 13,292.86%

**Payback Period**

= ($175,000/$23,437,500) x 12

Payback Period = 0.09 months

Approximately 2.7 days using a 30-day month.

---

## Task 4.3 Multi-Factor Authentication Enhancement

**Initial Investment**

= $200,000

**Annual Maintenance**

= $30,000 per year

**Risk Reduction (in $)**

Current ALE = $3,000,000

Control Effectiveness = 95%

= $3,000,000 × 0.95

Risk Reduction = $2,850,000

**Return on Investment (ROI)**

First-Year Total Cost:

= $200,000 + $30,000 = $230,000

ROI = (($2,850,000 - $230,000)/$230,000) x 100

ROI = 1,139.13%

**Payback Period**

= ($230,000/$2,850,000) x 12

Payback Period = 0.97 months

Approximately 29.1 days using a 30-day month.

### Summary of Cost-Benefit Analysis

| Metric | Advanced API Gateway | WAF | MFA Enhancement |
|----------|----------|----------|----------|
| Initial Investment | $350,000 | $150,000 | $200,000 |
| Annual Maintenance | $50,000 | $25,000 | $30,000 |
| Risk Reduction | $675,000 | $23,437,500 | $2,850,000 |
| ROI | 68.75% | 13,292.86% | 1,139.13% |
| Payback Period | 7.11 months | 0.09 months | 0.97 months |

## Task 5: Control Selection Analysis

### Task 5.1 Create a Scatter Plot Showing Cost vs. Effectiveness of Controls

