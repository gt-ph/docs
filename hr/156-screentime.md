---
title: "ScreenTime - ScreenTime"
description: "A centralised platform that streamlines supplier onboarding by automating data collection for security and technical clearances."
sidebarTitle: "ScreenTime"
icon: "users"
---

# ScreenTime - ScreenTime

| Field | Value |
| --- | --- |
| Requested team | Screen Time |
| Judging group | Final Judging Group 1 |
| Scheduled time | 1:20pm |
| Team number | 156 |
| Category | HR |
| Booth | 10B-10 |
| Project page | [https://build.tech.gov.sg/projects/2026/156](https://build.tech.gov.sg/projects/2026/156) |
| Product link | [https://screentime-v2.cio.sandbox.gov.sg/](https://screentime-v2.cio.sandbox.gov.sg/) |
| Team members | Chee Hui Hon; Jason Cheah; Jeffrey Choy; Jennifer Lai |

## Summary

A centralised platform that streamlines supplier onboarding by automating data collection for security and technical clearances.

## Full Write-Up

# Problem Statement
## Users
1.    Government officer(s)
  Contract Managers
  Project teams
  Agencies HR(s)
  Agencies Admin(s)
2.   Supplier(s)
## Use Case
Government officers in government agencies need to onboard supplier personnel quickly and compliantly before work can begin. This occurs at the start of every project and whenever new team members are added and is typically managed manually across email and Excel.
The current process is fragmented and inefficient for both government officers and suppliers. For security clearance, officers manually collect supplier data via email, reformat it into a standardised MHA template, and submit a task that takes 1 to 2 hours per submission. For technical clearance, suppliers submit personnel qualifications via email for assessment against project requirements. In both cases, errors in submission trigger back-and-forth exchanges, causing delays of up to 1 to 2 weeks. With no centralised system to track or manage process, the administrative burden for both officers and suppliers is high, oversight is limited and the risk of error is significant.
## Pain Point
1. Administrative Burden & Dual-Template Complexity
  The official MHA template contains internal-only columns unsuitable for external sharing, forcing government officers to maintain two separate templates, one simplified version for suppliers, one official version for submission. This dual-template approach creates unnecessary reformatting work and increases the risk of data inconsistencies between versions. For technical assessment, a similar issue exists, there is no centralised system to submit personnel qualifications, leading government officers to manually consolidate and reformat submissions to meet assessment requirements.
1. Repetitive Manual Data Entry
  Each security screening submission requires government officers to manually copy data from the supplier's simplified template into the official MHA template, the process could take 1–2 hours per submission depending on the quality and quantity of the submission. For technical assessment, government officers must similarly extract and consolidate qualification records for assessment. With resources onboarded progressively under procurement arrangements like Bulk Tender 24014, this cycle repeats multiple times across a project's lifecycle, compounding the administrative burden. Suppliers face an equally repetitive process, re-preparing and resubmitting personnel data and qualifications for every new project engagement, regardless of prior submissions.
1. Error-Prone Coordination
  Incomplete or incorrect submissions trigger back-and-forth exchanges between government officers, system integrators, and suppliers to obtain corrections, extending screening timelines by 1–2 weeks, particularly when multiple personnel require corrections simultaneously. From the supplier's perspective, the absence of real-time feedback means errors are only surfaced after submission, making it difficult to resolve issues promptly and delaying their personnel's mobilisation.
1. Data Security & Compliance Risks
  Transmitting sensitive personal data (NRIC, family details) via email creates unnecessary exposure to data leakage. The absence of a centralised tracking system also means government officers must manually monitor clearance statuses and submission records across projects, increasing the risk of lost documentation and compliance gaps.
1. Redundant Screening Across Agencies
  Despite over 80% of screenings returning positive results, supplier personnel are required to resubmit credentials for every new project, even when they have recently completed similar work at other agencies. The lack of cross-agency data sharing means the same screening effort is duplicated repeatedly, with no mechanism to recognise prior clearances.
## Consequence
1. Escalating Administrative Costs
  Without addressing these inefficiencies, administrative overhead will continue to compound as government digitalization projects increase. Government officers will spend progressively more time on manual processes, diverting resources from strategic project activities. For suppliers, the burden is equally significant, staff must repeatedly prepare and resubmit documentation, consuming time that could otherwise be directed towards project delivery. The 1 to 2 hours per individual submission will multiply across agencies, creating significant opportunity costs and reducing overall productivity in government technology initiatives.
1. Project Delivery Delays
  Persistent 1 to 2 week delays per submission accumulate across a project's lifecycle, particularly where resources are onboarded progressively. For time-sensitive government initiatives, these delays can push back project starts, disrupt downstream workstreams, and in some cases cause cascading effects on interdependent public-facing services, directly impacting citizens who depend on timely delivery. For suppliers, these delays directly affect their ability to mobilise personnel on time, disrupting project planning and resource allocation.
1. Heightened Security & Compliance Risk
  Continued transmission of sensitive personal data such as NRIC numbers, family details via email creates growing exposure to data breaches and privacy violations. As cyber threats evolve, this risk intensifies. A breach involving supplier personnel data could result in regulatory penalties, reputational damage to the agencies involved, and erosion of public trust in government data handling, consequences that far outweigh the cost of fixing the process.
1. Systemic Inefficiency Across Government
  Left unaddressed, this inefficiency will replicate itself across every agency running supplier-involved projects. With over 80% of screenings returning positive results and no mechanism to recognise prior clearances, the same redundant effort is duplicated government-wide directly undermining Singapore's broader public sector digitalisation goals and the push toward leaner, smarter government operations.
# User Research and Market Analysis
## User Research
Conducted surveys on suppliers and government officers, with 25 responses:
1. Surveyed government officers reported having 1 to 5 submissions per month and spending an average of 1.5 hours per submission on the current process.
1. 40% of government officers and suppliers experienced project timeline delays directly caused by security clearance delays
1. Over 50% of government officers confirmed that more than half of submissions contain errors requiring follow-up
1. All surveyed suppliers confirmed they had experienced at least one resubmission request
Prototype Testing (During Feedback Bazaar):
1) 82% of evaluators agreed that the product solves a real, significant pain point effectively, with an average rating of 4.5 out of 5.
2) 80% of evaluators agreed that the solution warrants further development and investment, with an average rating of 4.4 out of 5.
3) 76% of evaluators were highly impressed by the team's execution and the quality of the demo, with an average rating of 4.2 out of 5.
4) Evaluators highlighted the solution's relevance for both G50 and CAT2 security clearance processes as a strong use case, with the auto-generation of templates cited as a particularly valuable feature.
5) Evaluators also suggested expanding the solution's scope beyond vendor clearance to include other use cases such as visitor screening for prisons and new hire onboarding.
## De-risking
1. Change Management — Relearning a new process
  Adopting a centralised platform requires both government officers and suppliers to adapt to new workflows, which may initially slow adoption. For government officers, this is mitigated through structured onboarding that includes user guides, training walkthroughs, and a helpdesk channel. Government officers handling technical assessments will receive dedicated training on submitting, reviewing, and tracking qualification records within the platform. Suppliers will be supported through clear submission guidelines, annotated templates, and a dedicated support channel covering both security screening and technical assessment processes. The platform will be piloted with 1–2 agencies to surface friction points before wider rollout, with agency-level champions designated to drive adoption and provide peer support throughout the transition.
1. Trust — Decentralised responsibility leading to misuse
  With multiple agencies, government officers, and suppliers accessing the platform, there is a risk of unauthorised data access or misuse of sensitive personnel information. This is mitigated through role-based access controls, ensuring each user can only view and action data relevant to their role — suppliers are restricted to their own personnel's data, while qualification records and assessment outcomes are accessible only to authorised officers and relevant project teams. A full audit trail will log every submission, data access, and status update, maintaining clear accountability. Periodic compliance checks and clear accountability guidelines will further reinforce responsible use across all user groups.
1. Demand — Fluctuating Utilisation
  Fluctuating utilisation across security screening and technical assessments both tied to project milestones and onboarding cycles rather than steady activity may create the perception that the platform is underutilised during quieter periods. Irregular submission volumes may also affect suppliers' familiarity and confidence in the platform over time. These risks are mitigated by establishing clear usage metrics and reporting that contextualise demand patterns across the project lifecycle, demonstrating that lower activity reflects natural project rhythms rather than low adoption. Realistic utilisation benchmarks set during the pilot phase will manage stakeholder expectations, while periodic communications will sustain supplier engagement between peak periods.
1. Data Security & Compliance — Handling Sensitive Personnel Data
  Centralising sensitive personnel data including NRIC numbers, family details, professional qualifications, and project-specific records, introduces risks around data breaches, unauthorised access, and regulatory non-compliance. Suppliers may also have concerns about how their personnel's data is stored, shared, and retained on a government-managed platform. These risks are mitigated through end-to-end encryption, strict data retention policies, and compliance with the Personal Data Protection Act (PDPA) and relevant government data security standards. Transparent data governance policies will be communicated clearly to suppliers to build confidence, supported by regular security audits and clear escalation pathways in the event of a data incident.
## Stakeholder Buy-in
(Have yet to discuss with relevant stakeholder in supporting the POC post-hackathon, will add in after)
# Solutioning
## Problem-Solution Fit
A centralised digital platform that enables supplier personnel and government officers to self-service their onboarding by automating and redesigning submission workflows for both security and technical clearances.
## Functionality
Supplier Flows
1. Request Submission: Supplier logs into the platform and initiates a security clearance or technical assessment request through a guided, step-by-step form with inline validation to minimise errors before submission.
1. Status Tracking: Supplier accesses a personalised dashboard to monitor the status of all submitted requests in real time, replacing the need to follow up via email.
1. Clarification Response: Where the government officer requires additional information, the supplier receives an in-platform notification and can respond directly without reverting to email.
1. Result Notification: Supplier is automatically notified of clearance or assessment outcomes upon release, with clear next steps where applicable.
Government Officer Flows
1. Dashboard Overview: Upon login, officers are presented with a unified dashboard summarising all active clearance and technical assessment requests, outstanding actions, and clearance statuses across all supplier personnel.
1. Request Review & Clarification: Officers can review submitted requests, flag incomplete or incorrect entries, and raise clarification requests directly to the supplier within the platform.
1. MHA Template Export: Once validated, officers can export submission-ready data automatically mapped to the official MHA-formatted template, eliminating manual reformatting.
1. Result Update: Upon receiving clearance outcomes from MHA, officers update the platform to reflect results, triggering automatic supplier notification.
1. Technical Assessment Management: Officers review technical assessment submissions and record assessment outcomes directly within the platform, maintaining a centralised record across all projects.
## User Experience
The platform eliminates manual reformatting through integrated MHA template generation, provides real-time submission tracking and error validation to prevent delays, and offers a unified dashboard for officers and suppliers to manage the entire onboarding process. By digitising these fragmented manual processes, the platform reduces officer processing time from 1-2 hours to minutes per submission, cuts project delays caused by clearance bottlenecks, and minimises the resubmission cycles that currently affect 100% of suppliers.
## User Validation
(Have yet to conduct user testing with prototype at this point, will add in after)
# Impact & Next Steps
## Success Metrics
Reduce end-to-end supplier onboarding time from hours to minutes. Enabling government officers and suppliers to onboard personnel faster, with fewer errors, less administrative overhead, and full compliance confidence.
## Expected Impact
1. Faster Onboarding
  Reduction in submission preparation time from 1–2 hours to under 15 minutes per security submission with an estimated 85% reduction in preparation time. For technical assessments, centralised consolidation of qualification records is expected to reduce assessment turnaround time by at least 50%. Both government officers and Suppliers benefit from a streamlined submission process, and faster onboarding.
1. Fewer Errors & Re-submissions
  Structured data collection and automated template generation are expected to reduce submission error rates to near zero for security screening, eliminating the current 1–2 week correction delays. For technical assessments, standardised qualification submission formats are expected to reduce erroneous or incomplete submissions by 80%. Suppliers gain clarity on submission requirements upfront, targeting a reduction in back-and-forth correction exchanges from an average of 2–3 rounds to zero.
1. Reduced Administrative Burden
  Government officers are expected to reclaim 1–2 hours per security screening submission and 2–3 hours per technical assessment cycle previously spent on manual data re-entry and email coordination — time that can be redirected towards higher-value project delivery activities. Across a project lifecycle with multiple onboarding cycles, this translates to a significant cumulative reduction in administrative overhead per government officers and supplier.
1. Improved Data Security Compliance
  Sensitive personal credentials (NRIC, family details, professional qualifications) are no longer transmitted via email, reducing exposure to data breaches and strengthening compliance with data protection requirements.
1. Centralised Visibility
  Government officers gain a single source of truth for screening statuses across all submissions, eliminating the need for manual tracking across emails and spreadsheets and reducing time spent on status follow-ups. Suppliers gain real-time visibility into submission statuses, targeting a reduction in follow-up and re-submission exchanges enabling more confident and timely resource planning and deployment.
## Pitching Deck
https://gccprod-my.sharepoint.com/:p:/g/personal/jason_cheah_customs_gov_sg/IQDWHU5sT3U9SJguO7p98rCnAZzERtuShPPlenvdUEKCa3E?e=A8Qal8
