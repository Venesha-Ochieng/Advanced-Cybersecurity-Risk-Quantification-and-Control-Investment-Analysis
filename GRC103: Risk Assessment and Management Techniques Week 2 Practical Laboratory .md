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
![Task 5.1 - Cost vs Effectiveness](task%205.1.png)

### Interpretation

MFA Enhancement has the highest stated effectiveness (95%) at $230,000 first-year cost. WAF costs the least ($175,000) and has 75% stated effectiveness. API Security Gateway costs $400,000 and has 90% stated effectiveness. Effectiveness percentages alone cannot determine value because the controls mitigate risks with different starting ALEs.

## Task 5.2 Generate a Bar Chart Comparing ROI for All Controls
![Task 5.2 - ROI Comparison](task%205.2.png)

### Interpretation

WAF has the highest modeled ROI (13,292.86%) because it is applied to the database-injection risk, which has the largest baseline ALE ($31.25 million). MFA Enhancement follows at 1,139.13%, then API Security Gateway at 68.75%. Each control has a positive modeled first-year ROI.

## Task 5.3 Develop a Line Graph Showing Risk Reduction Over Time

Since the scenario gives no deployment dates, the implementation schedule below is illustrative: API Gateway becomes effective in Month 1, MFA in Month 2, and WAF in Month 3. The displayed figures represent annualized exposure at each milestone, not cash losses accrued during that month.

| Month | Milestone | Annual reduction achieved | Remaining annual ALE |
|---------|----------|--------------------------|----------------------|
| 0 | Baseline | $0 | $35,000,000 |
| 1 | API Gateway | $675,000 | $34,325,000 |
| 2 | MFA Enhancement | $3,525,000 | $31,475,000 |
| 3 | WAF | $26,962,500 | $8,037,500 |
| 6, 9, 12 | Monitoring / reassessment | $26,962,500 | $8,037,500 |

![Task 5.3 - Risk Reduction Timeline](task%205.3.png)

### Interpretation

The largest decrease occurs once WAF becomes effective in Month 3. Combined modeled annual exposure falls from $35 million to $8.0375 million, a reduction of $26.9625 million (77.04%). The flat period from Month 3 onward assumes unchanged threat conditions and sustained control effectiveness.

# Phase 3: Executive Reporting

**Organization:** SecureBank Financial  
**Platform:** SecureMobile Banking Application  
**Prepared by:** GRC Analyst  
**Reporting Period:** Annual Risk Assessment

## 6.1 Executive Summary

The cybersecurity risk assessment of SecureBank Financial's SecureMobile banking application identified three significant vulnerabilities: Database Injection, Session Hijacking, and API Authentication Bypass. These vulnerabilities present a combined estimated Annualized Loss Expectancy (ALE) of $35,000,000.

To mitigate these risks, the assessment recommends implementing a Web Application Firewall (WAF), Multi-Factor Authentication (MFA) Enhancement, and an Advanced API Security Gateway.

The proposed controls require an initial investment of $700,000 and annual maintenance of $105,000, resulting in a combined first-year cost of $805,000. Under the assumptions, these controls are projected to reduce annual risk exposure by $26,962,500 (77.04%), leaving a residual ALE of $8,037,500.

## 6.2 Top Three Cybersecurity Risks and Financial Impact

| Risk | Current ALE | Residual ALE | Priority |
|------|-------------|--------------|----------|
| Database Injection | $31,250,000 | $7,812,500 | Critical |
| Session Hijacking | $3,000,000 | $150,000 | High |
| API Authentication Bypass | $750,000 | $75,000 | Medium |
| Total | $35,000,000 | $8,037,500 | |

## 6.3 Recommended Security Controls and Costs

| Recommended Control | Initial Investment | Annual Maintenance | First-Year Total |
|--------------------|-------------------|-------------------|------------------|
| Web Application Firewall | $150,000 | $25,000 | $175,000 |
| MFA Enhancement | $200,000 | $30,000 | $230,000 |
| Advanced API Gateway | $350,000 | $50,000 | $400,000 |
| Total | $700,000 | $105,000 | $805,000 |

## 6.4 Expected Risk Reduction and ROI

| Security Control | Annual Risk Reduction | First-Year ROI |
|------------------|----------------------|----------------|
| Web Application Firewall | $23,437,500 | 13,292.86% |
| MFA Enhancement | $2,850,000 | 1,139.13% |
| Advanced API Gateway | $675,000 | 68.75% |
| Combined | $26,962,500 | 3,249.38% |

The combined ROI is calculated using total projected risk reduction and combined first-year costs, rather than adding the individual ROI percentages.

Overall ROI = ((26,962,500 - 805,000) / 805,000) x 100

Overall ROI = 3,249.38%

## 6.5 Required Visualizations and Interpretation

### 6.5.1 Risk Exposure Before and After Controls
![Task 6.5.1 - Risk Exposure](task%206.5.1.png)

Database injection declines from $31.25 million to $7.8125 million. Session hijacking declines from $3 million to $150,000, and API bypass from $750,000 to $75,000. Database injection still drives the bulk of residual exposure, warranting further remediation and validation.

### 6.5.2 Control Investment Breakdown
![Task 6.5.2 - Investment Breakdown](task%206.5.2.png)

The API Security Gateway has the greatest first-year cost ($400,000), followed by MFA ($230,000) and WAF ($175,000). Initial cost totals $700,000 and maintenance adds $105,000.

### 6.5.3 ROI Comparison Across Controls
![Task 6.5.3 - ROI Comparison](task%206.5.3.png)

## 6.6 Executive Recommendations

Based on the quantitative risk assessment and cost-benefit analysis, the following actions are recommended:

1. **Prioritize Database Injection Remediation:** Implement the WAF alongside secure coding improvements, parameterized queries, vulnerability patching, and application security testing.

2. **Strengthen Customer Authentication:** Deploy MFA Enhancement together with secure session management controls to reduce unauthorized account access and account takeover risks.

3. **Improve API Security:** Implement the Advanced API Security Gateway to strengthen authentication, authorization, transaction validation, and monitoring.

4. **Establish Continuous Risk Monitoring:** Monitor control effectiveness, track residual risk exposure, and report material changes to the CISO and executive management.

5. **Approve the Proposed Security Investment:** Consider approving the $805,000 first-year control budget, subject to technical feasibility, validation of the financial assumptions, and formal risk acceptance procedures.

## 6.7 Conclusion

The executive dashboard demonstrates the potential financial and security benefits of implementing the proposed cybersecurity controls across SecureBank Financial's SecureMobile banking platform.

The combined investment of $805,000 is projected to reduce annualized financial risk exposure from $35 million to approximately $8.04 million, representing a 77.04% reduction and a modeled first-year ROI of 3,249.38%.

The Web Application Firewall offers the greatest projected financial risk reduction, while MFA Enhancement and the Advanced API Security Gateway provide additional protection against account takeover and unauthorized transactions.

The CISO and CFO should prioritize approval and implementation of the recommended controls, supported by continuous monitoring, vulnerability remediation, and periodic evaluation of residual cybersecurity risk.

## Task 7: Risk Treatment Timeline
![Task 7 - Gantt Chart](task%207.png)

| Milestone | Success Indicator | Accountable Owner |
|------------|------------------|-------------------|
| Day 30 | Critical exposures contained and remediation plan approved | CISO |
| Day 90 | Three proposed controls deployed and validated | Head of Security Engineering |
| Month 6 | Control effectiveness reviewed and outstanding findings tracked | GRC Manager |
| Month 12 | Annual reassessment completed and residual risks reported | CISO |

## References

1. Idris, A. (n.d.). *Study guide: Quantitative risk calculations for GRC professionals (Course study guide).*
