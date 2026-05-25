---
title: "The CTRLs - Project ReView"
description: "How can we enable citizens to control how their data are used by AI in automated decision making or service completion?"
sidebarTitle: "The CTRLs"
icon: "users"
---

# The CTRLs - Project ReView

| Field | Value |
| --- | --- |
| Requested team | The CTRLs |
| Judging group | Final Judging Group 2 |
| Scheduled time | 2:03pm |
| Team number | 311 |
| Category | Data & AI |
| Booth | 9C-09 |
| Project page | [https://build.tech.gov.sg/projects/2026/311](https://build.tech.gov.sg/projects/2026/311) |
| Team members | Elise Robinson; Georgia Rajamanoharan; Leo Zhao; Maxwell Riess; Ming Sien Choong; Monica Crusellas; Richard Eveson; Sachin Tonk |

## Summary

How can we enable citizens to control how their data are used by AI in automated decision making or service completion?

## Full Write-Up

# Problem Statement
## Users
Who are the people affected? Include the size/quantity of users affected if possible.
- Citizens receiving AI-assisted government decisions, including welfare assessments, benefit claims, and healthcare entitlements
- Any individual whose personal data contributes to an automated or AI-assisted public service outcome
## Use Case
What are they trying to do and what task are they trying to complete? Where and when do they encounter this problem?
- A citizen submits an application or claim. An AI-assisted system retrieves personal data, such as health, employment, or financial records, to support a recommendation or decision. The citizen receives an outcome, but has little visibility into:
  - What data was used,
  - How AI contributed to the decision, or
  - How to challenge the outcome effectively
With increasing integration of AI into the delivery of government, citizens need to understand when their data is used and have control mechanisms over the use of that data.
Given a future automated government service journey, e.g. applying for a benefit, citizens should have the agency to control how their data are used, and the agency to complete a journey without their data being used by an AI system altogether if desired.
How do we design user journeys that provide control to the citizen over their data? How do we engineer automated AI systems with this level of control “baked in”?
## Pain Point
What is the possible root cause behind the problem you have observed?
- Government AI systems often operate under statutory data-sharing powers rather than individual consent. While legally permitted, this can create a lack of transparency and user agency.
- Today, citizens typically receive only the final outcome, with limited explanation of:
  - What information informed the decision,
  - What role automation played, or
  - What review options exist.
  This makes it difficult for the citizen to identify incorrect data, request human review, or meaningfully contest the decision.
Citizens can be unclear on where and how their data are used in interactions with government systems, particularly in AI systems and decision making. They may perceive that they do not have control over when their data are used, and they may have misunderstandings or lack of knowledge on how sharing of that data could be beneficial in helping better decision making, and whether an AI system can be safely relied on to make a decision.
## Consequence
What happens if we don't solve the problem? Size your consequence based on the magnitude of effect on your users.
- This is an inevitable problem that will only grow with time as more government digital services are digitalized, and AI is increasingly integrated into their workflows.
- Without clear transparency and contestation pathways:
  - Erroneous decisions may go unchallenged,
  - Trust in AI-assisted public services declines, and
  - Departments face increasing scrutiny around compliance, accountability, and explainability obligations.
Citizens lack meaningful understanding, control, and recourse over how their data are used in automated or agent-led decisions, limiting trust, accountability, and their ability to influence outcomes that affect them.
# User Research and Market Analysis
## User Research
What user research methods did you adopt to validate that this solution is needed and what were the key insights from real users?
- We are still conducting user testing to validate our assumptions.
- Current validation questions:
  - Do citizens value granular consent, or experience it as friction?
  - What level of explanation builds trust without overwhelming users?
  - Do users understand different contestation routes (data issue vs AI objection vs outcome disagreement)?
  - How do users respond to just-in-time consent prompts?
## De-risking
What market risks are there and how did you mitigate them?
- Consent fatigue: Mitigated by a hybrid model — upfront category-level defaults plus single just-in-time confirmation per category per session, not per query.
- Graceful degradation: Agent is architected to produce partial assessments when consent is withheld, rather than failing — preventing consent from becoming a barrier to service access.
- Prompt injection: Enforcement is implemented in the Python tool wrapper, not in the AI prompt — injected instructions in retrieved records cannot override consent gates.
- Legal basis: The system is designed to support both explicit consent and substantial public interest as legal bases, surfacing the applicable basis to the citizen before processing begins.
## Stakeholder Buy-in
Which agencies or departments did you reach out to and did they express interest or commitment?
- TBC. We are still conducting user testing to determine product-market fit.
# Solutioning
## Problem-Solution Fit
How does your product specifically address the pain points identified?
- It addresses two core gaps in AI-assisted public services:
  - Lack of meaningful user control over data usage
  - Lack of transparency and contestability after a decision is made
- The prototype combines:
  - Consent-aware data access controls, and
  - Structured decision receipts with integrated contestation pathways.
## Functionality
What are your key user flows/features?
- Consent Cards: Plain-language consent cards explain:
  - What data will be accessed,
  - Why it is needed, and
  - What happens if consent is denied.
  Sensitive categories (e.g. mental health records) require
separate confirmation.
- Just-in-Time Confirmation: Consent prompts appear immediately before data retrieval, once per category per session, balancing transparency with usability.
- Three-Layer Consent Enforcement: Consent is enforced across three layers:
  - Tool-level Python wrapper checks the consent registry before any retrieval executes
  - Non-consented tools are not registered in the agent's tool list at all
  - System prompt informs the agent of the current consent state to avoid futile calls.
  Layers 1 and 2 are enforced in code and cannot be overridden by the model.
- Decision Receipt: A structured, progressively disclosed explanation of:
  - The decision outcome,
  - Key contributing factors,
  - Data used,
  - Role of AI,
  - Human review points, and
  - Next steps.
  The receipt also functions as an auditable interaction log.
- Contestation Pathways: Users can:
  - Dispute the outcome,
  - Challenge incorrect evidence, or
  - Object to AI involvement.
  Each route gathers structured inputs and directs the case to the appropriate review pathway.
Contestation Pathways: Users can:
Dispute the outcome
- Mid-Session Revocation: Users can withdraw consent during the session. Retrieved data is removed from the agent’s active context, not just blocked from future access.
## User Experience
How did you make the experience seamless/intuitive for the end user?
- The UI uses progressive disclosure throughout:
  - Simple summaries first,
  - Deeper detail only when needed.
- The goal is to make explanation actionable without overwhelming users.
- The contestation flow is integrated directly into the service journey, rather than treated as a separate appeals process.
## User Validation
What feedback did users give about the product? What worked well and what required improvement?
- TBC. We are still conducting user testing.
# Impact & Next Steps
## Success Metrics
What is your "North Star" metric?
- Citizen trust in AI-assisted government decisions measured by the proportion of users who, having received a decision, report that they understand how it was reached and feel confident they could contest it if needed.
## Expected Impact
What outcomes do you expect this to be able to deliver in the short/medium/long term if your product is launched to users?
- Short Term:
  - Demonstrates that:
    - Granular consent enforcement,
    - Structured explanation, and
    - Contestation pathways
    can be operationalised within AI-assisted government services.
- Medium Term:
  - Provides reusable infrastructure for:
    - Decision transparency,
    - Auditability, and
    - Structured review workflows.
  - Supports emerging accountability and documentation requirements, including ATRS-aligned records.
- Long Term:
  - Establishes a reusable trust and transparency layer for citizen-facing government AI services.
  - Serves as a practical model for operationalising explainability, accountability, and contestability rights in public-sector AI.
Appendix: Regulatory Context
Singapore and the UK share similar high-level approaches to AI governance:
- Data protection law as the enforcement backbone,
- Layered AI governance guidance, and
- A pro-innovation regulatory posture.
Both frameworks emphasise:
- Transparency,
- Accountability,
- Proportionate human oversight, and
- Citizen rights around personal data usage.
Relevant Singapore frameworks:
- Personal Data Protection Act 2012 (PDPA)
- PDPC Advisory Guidelines on AI Recommendation and Decision Systems (2024)
- Model AI Governance Framework
Relevant UK frameworks:
- UK GDPR / Data Protection Act 2018
- ICO Guidance on AI and Data Protection
- Algorithmic Transparency Recording Standard (ATRS)
Key Difference:
- UK GDPR Article 22 explicitly provides a right relating to solely automated decision-making and human review.
- Singapore’s PDPA does not currently contain an equivalent statutory right.
Where The Product Fits:
- Operationalises transparency and contestability at the transaction level:
  - Making AI-assisted decisions more legible,
  - Enabling structured challenge pathways, and
  - Improving citizen visibility into how personal data shapes outcomes.
