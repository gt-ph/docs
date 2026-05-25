---
title: "RAMP - RAMP (Risk Acceptance Management Platform)"
description: "A guided risk acceptance platform that turns scattered inputs into traceable, renewable risk decisions with one structured review and approval flow."
sidebarTitle: "RAMP"
icon: "users"
---

# RAMP - RAMP (Risk Acceptance Management Platform)

| Field | Value |
| --- | --- |
| Requested team | RAMP |
| Judging group | Final Judging Group 3 |
| Scheduled time | 1:53pm |
| Team number | 69 |
| Category | Cybersecurity |
| Booth | 8B-07 |
| Project page | [https://build.tech.gov.sg/projects/2026/69](https://build.tech.gov.sg/projects/2026/69) |
| Product link | [https://rampv4.cio.sandbox.gov.sg/](https://rampv4.cio.sandbox.gov.sg/) |
| Team members | Kelly Tan From.tp; Nelson Yy Chin; Raymond Lee; Wang Hao Lee; Woei Shyang Siaw |

## Summary

A guided risk acceptance platform that turns scattered inputs into traceable, renewable risk decisions with one structured review and approval flow.

## Full Write-Up

# Problem Statement
## Users
Approximately 200 GovTechies across 50+ government agencies who participate in risk acceptance – as submitters (Product/Project Managers, Technical Specialists), reviewers (ACISO/MCISO), approvers (CIO/CTO/IDSC), governance coordinators, or business owners of affected systems. The pain is shared across the chain, not concentrated in one role.
## Use Case
GovTechies are required to obtain formal risk acceptance through multiple channels and documentation methods when implementing new technologies or systems. The current process involves several approaches, including composing detailed email communications with comprehensive risk assessment documents attached in Word format, or utilising the organisation's intranet-based risk management system for formal submissions.
## Pain Point
Each GovTechie spends 12–15 hours per month navigating risk acceptance procedures. Every time a risk assessment needs approval, they have to individually prepare documentation across up to 4 different formats and submission channels - drafting formal emails, creating Word document attachments, logging into separate intranet systems for different risk categories, and following up with multiple stakeholders across cybersecurity, project management, and data governance teams, in addition to responding to individual clarification requests and resubmitting documentation when requirements differ between approval authorities.
## Consequence
This results in up to 6,000 man-hours (15 hours x 200 GovTechies x average 2 iterations) per month spent on risk acceptance procedures across the organisation – valuable time taken away from core technology development and implementation activities.
# User Research and Market Analysis
## User Research
What user research methods did you adopt to validate that this solution is needed and what were the key insights from real users?
We synthesised 42 feedback notes collected from active participants in the risk acceptance process across submitters, reviewers and approvers. The notes were analysed for recurring pain themes, role-based segmentation and behavioural patterns to validate the problem and shape product priorities.
Three dominant user groups emerged from the feedback:
[table block omitted in flat markdown; see narrativeBlocks in JSON]
Top recurring pain themes (ranked by mention count) confirmed that the problem is not just submission friction – it is the substantive difficulty of producing a defensible risk acceptance:
[table block omitted in flat markdown; see narrativeBlocks in JSON]
From these themes we derived six core personas, each anchored to a distinct Job-to-be-Done. The most material insight is that today’s pain is shared across submitters, reviewers, approvers, governance coordinators and business owners – a pure submission portal would only serve one slice:
[table block omitted in flat markdown; see narrativeBlocks in JSON]
A second-layer behavioural analysis surfaced an adoption insight that role-based personas alone could not: people respond to process friction differently. The starkest contrast is between users who have disengaged and those still pushing for reform. RAMP must win over the fatigued users while empowering the reform-minded ones:
[table block omitted in flat markdown; see narrativeBlocks in JSON]
Eight core Jobs-to-be-Done were prioritised from the research and now anchor the product backlog:
1. Define the risk clearly
1. Assess impact and likelihood properly
1. Identify valid mitigations
1. Submit through a clear approval workflow
1. Reduce approval delays
1. Maintain centralised evidence
1. Track expiry and lifecycle review
1. Make the process understandable for non-specialists
## De-risking
We mapped six categories of existing tools that touch parts of the risk acceptance job, and identified the white space RAMP must own:
[table block omitted in flat markdown; see narrativeBlocks in JSON]
Within the Enterprise GRC / IRM category, we conducted a deeper build-vs-buy comparison against the most prominent named platforms. Each offers something useful, but none is purpose-built for the specific GovTech job of guided risk-acceptance drafting, public-sector approval routing and renewal-delta visibility:
[table block omitted in flat markdown; see narrativeBlocks in JSON]
A consistent pattern emerges: enterprise GRC platforms are mature systems of record but expect users to already know how to write a defensible risk acceptance. RAMP’s opportunity is the guidance layer above the record – the assistance that turns scattered VAPT findings, vendor emails and business rationale into a coherent decision narrative that an ACISO, CIO or IDSC member can act on quickly.
From the broader analysis, three concrete adoption risks and our mitigations are:
- “Why not just buy a GRC platform?”
Enterprise GRC tools (ServiceNow GRC/IRM, Archer, MetricStream, OpenPages, SAI360, LogicManager) are strong as systems of record but weak at submitter guidance, plain-English decision narrative and public-sector approval routing. FedRAMP-friendly options like Onspring close the deployment gap but still require heavy configuration to fit GovTech’s specific workflow.
Mitigation: position RAMP as a guided lifecycle layer that consolidates the four existing channels, with AI-assisted drafting, mitigation adequacy scoring and renewal delta views – not as another GRC platform.
- Approver-behaviour risk
Even the cleanest submission portal will not reduce resubmission rates if approvers (cybersecurity, PMO, data governance) do not change how they review.
Mitigation: research surfaced approvers (Mr Lim persona) as a distinct user group with their own JTBD – “make confident decisions under time pressure.” RAMP includes a one-page approver brief, delta view and attention flags so approvers benefit from adoption, not just submitters.
- Adoption / workaround risk
The most concerning behavioural variant is The Senior Who Gave Up – users who treat any new system as one more layer unless it visibly removes work.
Mitigation: lead with work-reduction proof points (replace email + Excel + DGP duplication, reuse system context, auto-generate renewal summaries). Pair with The Senior Who Kept Going variant as in-agency champions to drive enforcement of one official workflow.
## Stakeholder Buy-in
Engagement and feedback have been gathered across the full risk acceptance chain, reflecting the multi-stakeholder map surfaced in the research:
- GovTech Risk Acceptance Team – favoured user class for format and decisioning standards.
- ACISO / MCISO reviewers – cybersecurity governance functions across ministries and agencies (12 of 42 feedback notes).
- CIO / CTO / IDSC approvers – senior accountable decision-makers (3 of 42 notes, but high-leverage).
- Governance / audit coordinators – lifecycle, evidence and renewal owners.
- Business / SaaS system owners – accountable for outcomes but often under-equipped on cyber vocabulary.
# Solutioning
## Problem-Solution Fit
RAMP is not another submission portal. The research showed that the highest-impact opportunity is to position RAMP as a risk acceptance lifecycle platform – covering submit → review → approve → monitor → renew → close, with a single source of truth across the four currently-fragmented channels (email + Word attachments, agency-specific risk systems, GitHub, intranet portals). This directly addresses the top three pain themes (mitigation proposal, impact/likelihood assessment, risk definition) by providing AI-assisted drafting, structured rating guidance and a reusable mitigation library, while solving the workflow pain (approval delay, audit evidence, lifecycle tracking) through auto-routing, central evidence capture and expiry alerts.
## Functionality
What are your key user flows/features?
- Guided risk drafting: wizard with AI-assisted risk statement, likelihood/impact and mitigation drafts; targets the top pain theme (32 mentions on alternative mitigations).
- Submission completeness check: AI pre-check before reviewer hand-off so weak drafts self-correct before reaching ACISO/MCISO (Aisha persona, addresses reviewer bottleneck).
- Auto-routing: submissions flow to the correct approver based on risk level, system classification and agency rules – removing manual chasing (Approval Chaser variant).
- Approver decision brief: one-page summary with risk, mitigation, residual risk, recommendation and delta-from-previous flags (Mr Lim persona). (Future roadmap)
- Lifecycle and renewal tracking: expiry alerts, version comparison, ownership continuity and audit-ready export (Mei persona).
- Reusable reference library: searchable repository of similar accepted risks and mitigation patterns, sanitised for cross-agency reuse.
- Plain-English decision summary: “what you are accepting” view for business owners (Marcus persona).
## User Experience
Three UX principles came directly out of the research. First, role-based views: submitters see a guided workspace, reviewers see a queue with ageing and SLA, approvers see a one-page decision brief, and governance coordinators see a lifecycle register – the same record, different lenses. Second, plain-English layer: the system translates risk severity, impact and mitigation language into business-friendly summaries so non-specialist business owners can approve confidently. Third, reuse over re-entry: system context (classification, hosting, tech stack) is captured once and persists across all future submissions, and prior accepted risks surface as suggestions rather than blank pages – directly addressing the Senior Who Gave Up variant’s demand for visible work reduction.
## User Validation
(Have yet to conduct full prototype testing at this point; will be added after the next round of validation sessions with the GovTech Risk Acceptance Team and a representative sample drawn from each of the six personas.)
# Impact & Next Steps
## Success Metrics
North Star: Hours per GovTechie per month spent on risk acceptance, reduced from 15 hrs to ≤3 hrs. A low number indicates RAMP is achieving meaningful time savings for the user base.
Supporting Tier-1 metrics:
[table block omitted in flat markdown; see narrativeBlocks in JSON]
## Expected Impact
- Short term: recover an estimated 2,400+ man-hours per month across the 200 GovTechies in scope (≈12 hours saved per user, per month) by collapsing the 4 submission channels into 1 structured flow.
- Medium term: faster delivery cycles across the 50+ agencies as approval friction drops and resubmission iterations fall from ~2 to ≤1; improved submission quality reduces ACISO/MCISO reviewer load.
- Long term: standardised risk-acceptance data unlocks cross-agency analytics on common risk patterns (CVEs, SaaS products, recurring scenarios), allowing the GovTech Risk Acceptance Team to anticipate and pre-empt frequently-recurring submissions, and giving senior leadership portfolio-level visibility of accepted risk concentration.
