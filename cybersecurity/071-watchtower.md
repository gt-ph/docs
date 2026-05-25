---
title: "WatchTower - WatchTower"
description: "High DLP alert volumes strain staff and cause alert fatigue. Intelligent triage mechanism is needed to prioritise alerts and reduce data leakage risk."
sidebarTitle: "WatchTower"
icon: "users"
---

# WatchTower - WatchTower

| Field | Value |
| --- | --- |
| Requested team | Watch Tower |
| Judging group | Final Judging Group 3 |
| Scheduled time | 2:23pm |
| Team number | 71 |
| Category | Cybersecurity |
| Booth | 8B-21 |
| Project page | [https://build.tech.gov.sg/projects/2026/71](https://build.tech.gov.sg/projects/2026/71) |
| Product link | [https://prod.gvt-build26-ai-dlp-analysis.prd.paas.sandbox.gov.sg/](https://prod.gvt-build26-ai-dlp-analysis.prd.paas.sandbox.gov.sg/) |
| Team members | David Hh Yeo; Guiyuan Ye; Irene Chan; Sathiyamoorthi Chinnasamy; You Jing Toh |

## Summary

High DLP alert volumes strain staff and cause alert fatigue. Intelligent triage mechanism is needed to prioritise alerts and reduce data leakage risk.

## Full Write-Up

# Problem Statement
## Users
Agency wide, Data Governance and Security Team
## Use Case
Agencies are required to review and follow up on all unfiltered DLP alerts across security, data, and business units. Given the sheer volume of alerts, manual triage involving multiple teams is humanly impossible. Without risk categorisation and prioritisation, it becomes difficult to decipher which alerts warrant more immediate attention for staff behaviour analysis. There is also no mechanism to track alerts or perform UEBA analysis at scale, compounded by the sensitivity of the data and privacy considerations around staff actions.
## Pain Point
There is no WoG-wide standard or tooling for intelligent, privacy-conscious DLP alert triage at scale. Existing platforms like Trellix fall short, offering insufficient granularity for effective UEBA without heavy, costly customisation.
Every month, agencies collectively face an avalanche of approximately 6,000,000 DLP alerts across 99 agencies. This staggering volume, combined with a low signal-to-noise ratio and limited contextual data, renders manual review not just impractical — but impossible. Genuine risks are buried under mountains of false positives, leaving agencies blind to real data loss threats.
Without risk categorisation and prioritisation, dangerous behaviours slip through undetected. The absence of an automated pipeline means stakeholders receive no timely, actionable insights. Poor data handling practices remain unaddressed, festering silently until they erupt into reputational or operational crises.
Today, monthly DLP alert reviews are treated as nothing more than a compliance checkbox. This is dangerously inadequate. In an era of accelerated AI adoption, alerts must evolve into real-time defences — proactive shields against insider threats.
## Consequence
The stakes are high. Legitimate data leaks are slipping through undetected or unresolved, exposing agencies to business, regulatory, and reputational risks.
At the same time, poor data handling continues unchecked, reducing DLP reviews to a compliance exercise rather than a meaningful defence.
Without stronger triage and actionable insights, agencies remain vulnerable to preventable insider threats.
# User Research and Market Analysis
## User Research
FormSG surveys were conducted across all CISOs in WoG to gather insights on DLP alert handling.
## De-risking
Agencies have distinct workflows and risk appetites, and a generalised solution risks low adoption if it fails to meet their specific needs. To mitigate this, the team will conduct user studies and polling sessions with representative agencies before and during development, with feedback loops maintained post-deployment. Adoption rates, proportion of agencies actively configuring custom rules, and user satisfaction scores will be used to measure whether this risk has been sufficiently addressed.
## Stakeholder Buy-in
We reached out to all agency CISOs via FormgSG to get feedback. Response was received from 9 agencies (AGO, CEA, JTC, MFA, MND, MSE, PMO, PMOSG, PUB), all of them have same pain points as MSF in handling the DLP alert monthly, only one agency used automation. This is a common WOG-wide gap, not a niche issue.
# Solutioning
## Problem-Solution Fit
The product supports agencies in meeting obligations around data protection and insider threat management by making DLP monitoring operationally sustainable at scale. By reducing alert fatigue and improving triage accuracy, it strengthens the agency’s ability to detect and respond to genuine data loss risks.
Importantly, the solution is designed with graduality — allowing each agency to adjust configurations and workflows according to their specific needs and risk appetite. This flexibility ensures adoption across diverse environments without forcing a one‑size‑fits‑all approach.
## Functionality
User flows/features for MVP as of now:
1) Ingestion of DLP Alert
2) Filter DLP Alert to show logs that is of concerns only, we are concentrating on alert of external storage, web upload and email that had potential risk of data leaking out as of current. Scoring criteria will be implemented based on condition to deem it low, medium and high risk for triage.
3) Include User Entity Behaviour Analysis to detect potential insider risk.
## User Experience
Agencies can easily upload DLP alerts, gain immediate visibility, and act on high‑risk alerts. With an AI‑driven UEBA core, correlation of alerts for insider risk is automatic.
The system’s graduality ensures agencies can start simple — filtering and scoring alerts — and progressively adopt advanced features like UEBA and custom rules as their maturity grows.
## User Validation
We intent to get feedback at the later stage for agencies that provided response over FormSG. We are using anonymized data from MSF DLP alert itself to work on the MVP now.
# Impact & Next Steps
## Success Metrics
Reduce number of false positive alerts by 50%
 
Reduce man days required for triaging by 99%
 
Staff data handling maturity through the tool’s reporting and awareness
## Expected Impact
Short Term:
Enable agency to filter out the false positive alert with our solution easily and only act on those true positive.

Medium Term:
Supports agencies in meeting their obligations around data protection and insider threat management by making DLP monitoring operationally sustainable at scale. By reducing alert fatigue and improving triage accuracy, it strengthens the agency's ability to detect and respond to genuine data loss risks. 

Long Term
Through our solution, we can easily identify staffs that need guidance on data handling and then introduce awareness training. The continual training for staffs that need guidance advances the broader objective of building a security-conscious workforce, addressing poor data handling practices at the source rather than purely through enforcement.
