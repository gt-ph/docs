---
title: "Unmute - OmniGov"
description: "OmniGov automates field data capture from WhatsApp/Telegram into audit-ready records, letting officers verify work at scale without manual data entry."
sidebarTitle: "Unmute"
icon: "users"
---

# Unmute - OmniGov

| Field | Value |
| --- | --- |
| Requested team | Unmute |
| Judging group | Final Judging Group 4 |
| Scheduled time | 2:56pm |
| Team number | 97 |
| Category | Communications and Engagement |
| Booth | 10D-02 |
| Project page | [https://build.tech.gov.sg/projects/2026/97](https://build.tech.gov.sg/projects/2026/97) |
| Product link | [https://omnigov.app.tc1.airbase.sg/](https://omnigov.app.tc1.airbase.sg/) |
| Team members | Adam Chee; Keith Choo; Kek Wei Chong; Keng How Lim; Yu Tung Chen |

## Summary

OmniGov automates field data capture from WhatsApp/Telegram into audit-ready records, letting officers verify work at scale without manual data entry.

## Full Write-Up

# OmniGov
#### Pitch
https://omnigov-pitch.cio.sandbox.gov.sg
#### 1. Problem Statement
- Users: Who are the people affected? Include the size/quantity of users affected if possible.

7 BCA Officers managing 50+ external contractors for the Private EASE (https://www.mnd.gov.sg/newsroom/press-releases/view/more-than-80000-eligible-households-to-benefit-from-the-enhancement-for-active-seniors-private-housing-programme) scheme. These 50+ contractors would service the 80k households eligible for the Private EASE scheme.
- Use Case: What are they trying to do and what task are they trying to complete? Where and when do they encounter this problem?

Officers must coordinate with contractors to verify Proof-of-Work (e.g., photo evidence of the gate with a timestamp metadata). Officers exercise judgment to guard against falsified submissions, such as the re-submission of duplicate photos from previous jobs or other units..
- Pain Point: What is the possible root cause behind the problem you have observed?

The workflow is fragmented across 7 individual business phones. This decentralization creates data silos, making it impossible to cross-reference photos for falsified submissions. Furthermore, because each chat is tied to a specific device, getting a colleague to cover for an absent officer requires a high-friction physical handover of the phone.
- Consequence: What happens if we don't solve the problem? Size your consequence based on the magnitude of effect on your users

The manual reconciliation process is highly labor-intensive, requiring one person to spend 2 to 3 hours daily manually tracking "OK/Ack" messages and photo sets against schedules.

The operations cannot scale as the scheme expands to the July tranche (Seniors 70-79) and the massive October peak (Seniors 65-69), which covers the bulk of the 80,000 eligible households.

Failure to automate will lead to "Verification Fatigue," where the risk of fraud and duplicate payouts increases as officers struggle to manually audit a 4x surge in unstructured chat data.
-
#### 2. User Research and Market Analysis
- User Research: What user research methods did you adopt to validate that this solution is needed and what were the key insights from real users?

We conducted direct observations of BCA's communication workflow, identifying a strong user preference for mobile-first interaction over web interfaces. Key insights revealed that while BCA staff prefer the native WhatsApp app for replies, management requires a high-level dashboard to "see what is inside" the chats without being added to every group.
- De-risking: What market risks are there and how did you mitigate them?

Sustainability & Scalability: A primary risk identified was that OmniGov might remain an expensive, "niche" solution limited to a single agency's workflow. To mitigate this, we conducted a scan to validate the reproducibility of the "Proof-of-Work" pattern. Our research identified the HDB Public EASE scheme as a high-potential parallel; it shares nearly identical operational DNA but at a significantly larger scale. By solving for BCA today, we are effectively stress-testing a solution that could be transplanted to the Public EASE scheme and other high-volume, field-verified government policies.
- Stakeholder Buy-in: Which agencies or departments did you reach out to and did they express interest or commitment?

BCA is interested in supporting the product.
#### 3. Solutioning
- Problem-Solution Fit: How does your product specifically address the pain points identified?

The existing chat would be integrated with our system, and is integrated with AI to parse the text and images, ensuring that the friction-free mobile workflow for contractors remains intact while the backend reporting is fully automated for the agency.
- Functionality: What are your key user flows/features?
  - Shared Inbox: Centralizes 50+ contractor threads into one dashboard, removing handover friction.
  - Productivity Dashboard: A real-time tracker sits alongside the inbox, automatically tallying "Work Completed" based on verified chat milestones. Officers can see at a glance the total volume of successful installations across all 7 business lines.
  - Augmented Extraction: An LLM parses "messy" chat logs into structured fields. We use a Human-in-the-Loop interface where officers "Verify & Commit" parse data with one click to prevent hallucinations.
  - Anti-Fraud Layer: The system automatically flags potential duplicate submissions by comparing new photos against a central database of historical entries across all 7 business lines.
- User Experience: How did you make the experience seamless/intuitive for the end user?

Minimise deviation from existing workflows where contractors continue using WhatsApp, while officers gain a "Single-Pane-of-Glass" view for all verifications.
- User Validation: What feedback did users give about the product? What worked well and what required improvement?

Have yet to conduct user testing with the prototype at this moment.
#### 4. Impact & Next Steps
- Success Metrics: What is your "North Star" metric?

Number of Verified Field Events Automatically Logged.
- Expected Impact: What outcomes do you expect this to be able to deliver in the short/medium/long term if your product is launched to users?
  - Productivity: Avoid manpower costs by enabling the 7-man team to handle the October volume surge without additional headcount.
  - Operational Resilience: Immediate removal of "Key Person Risk" through centralized data access.
