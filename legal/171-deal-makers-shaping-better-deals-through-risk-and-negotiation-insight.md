---
title: "Deal Makers - Shaping better deals through risk and negotiation insight. - Deal Makers"
description: "AI-powered ICT contract risk assistant that helps public officers identify, assess and escalate ICT contractual risks using GovTech playbooks."
sidebarTitle: "Deal Makers - Shaping better deals through risk and negotiation insight."
icon: "users"
---

# Deal Makers - Shaping better deals through risk and negotiation insight. - Deal Makers

| Field | Value |
| --- | --- |
| Requested team | Deal Makers |
| Judging group | Final Judging Group 3 |
| Scheduled time | 1:30pm |
| Team number | 171 |
| Category | Legal |
| Booth | 8A-02 |
| Project page | [https://build.tech.gov.sg/projects/2026/171](https://build.tech.gov.sg/projects/2026/171) |
| Team members | Aaron Ma; Desmond Oh; Yang Xi Wee; Zhenfa Ng |

## Summary

AI-powered ICT contract risk assistant that helps public officers identify, assess and escalate ICT contractual risks using GovTech playbooks.

## Full Write-Up

# Problem Statement
## Users
Public officers across Government involved in ICT procurement, contract review, project delivery, and SaaS onboarding — especially officers without regular legal or contract review experience.
## Use Case
Many public officers, especially product owners and ICT teams outside Procurement or Legal functions, do not review contracts regularly. Yet, they need to understand how ICT contracts, SaaS terms, EULAs, licensing agreements, and pricing schedules may affect operations, obligations, risks, and future options.

Officers may spend hours, or even up to a day or more, trying to understand a contract from scratch before engaging Procurement, Legal, or management. Deal Makers helps by providing a faster first-pass review, highlighting common commercial, legal, operational, and governance risks, explaining why they matter, and identifying issues for escalation, risk acceptance, or further review.
## Pain Point
Contract review requires specialised legal, commercial, and operational judgement, but many public officers only encounter ICT contracts occasionally. The knowledge of what to look out for is
often held by experienced Procurement, Legal, or senior officers, rather than embedded into a simple, consistent workflow. As a result, officers may struggle to identify which clauses matter, why they matter, and what should be escalated for further review.
## Consequence
If unaddressed, agencies may face avoidable cost escalation, hidden EULA exposures, and reduced negotiation leverage due to risks that are not identified early. Officers often rely on experience to navigate complex contract terms, leading to inconsistent risk assessment and missed opportunities to negotiate better outcomes. Over time, this results in higher ICT spending, repeated mistakes across agencies, and fragmented procurement practices—ultimately limiting Government’s ability to secure stronger, more consistent commercial terms at scale.
# User Research and Market Analysis
## User Research
We conducted prototype testing and qualitative user research with a cross-section of stakeholders across the ICT procurement ecosystem. Participants were deliberately selected to include ICT / technical teams who encounter vendor EULAs during implementation, procurement leaders / practitioners who assess contractual and commercial risks, and procurement policy stakeholders who understand broader WOG procurement considerations. This included inputs from IMDA CIO, MOE Tech Team, MOM Tech Team, HTX, DSTA and MOF.

This mix allowed us to validate the problem from multiple angles:
1. Whether ICT teams understand the operational risks in vendor terms,
1. Whether procurement teams can use the tool for first-cut risk assessment, and
1. Whether the concept has potential policy relevance if scaled across Government.
## De-risking
1. The key market risk is trust. Officers will not rely on a contract review tool if the outputs are generic, inaccurate, or not traceable to the actual clauses. To mitigate this, Deal Makers is built around GovTech-developed internal playbook, with each risk output linked to clause evidence, risk classification, explanation of consequences, and suggested mitigation actions. The tool is positioned as a first-pass informational aid, not a replacement for Legal, Procurement, or approving authority review.
1. A second risk is workflow adoption. Agencies already have established review and approval processes, so a standalone analysis tool may not be useful unless it helps officers move faster within those processes. To mitigate this, the prototype was refined based on agency feedback to include practical next-step outputs, such as Word report export and draft escalation emails to Legal or management for issues requiring further review.
1. A third risk is false positives or missed issues. User testing with IMDA, MOE, HTX and DSTA showed that users valued the structured risk review, but also highlighted the need for better clause referencing, improved coverage of issues such as liquidated damages and late payment, and clearer confidence indicators. These findings were used to improve the product design by adding clause traceability, confidence levels, and clearer “review required” labels where the tool is uncertain.
1. Finally, there is a governance risk if users misunderstand the tool as providing final legal clearance. To mitigate this, the product clearly frames outputs as indicative guidance, highlights areas for escalation or risk acceptance, and keeps human reviewers in the decision loop. This ensures the tool supports existing review processes while improving consistency, speed, and baseline awareness across officers.
## Stakeholder Buy-in
We reached out to a mix of ICT, procurement, and policy stakeholders across Government to validate whether the problem is real and whether the prototype would be useful in practice. This included ICT / technical stakeholders from IMDA CIO, MOE Tech Team and MOM Tech Team, procurement practitioners / leaders from HTX and DSTA, and procurement policy stakeholders from MOF.

The feedback received indicates clear interest in the use case, particularly as a fast first-cut review tool for ICT contracts, SaaS agreements, vendor EULAs and licensing terms. Agencies generally recognised that the tool could help officers identify potential risks earlier, understand risk severity, and know what issues to escalate for Legal, Procurement, technical or management review.

IMDA CIO shared that the app provides a “structured way to gather insights” and gives users “a good overview and a quick glance and appreciation of the risks”, while noting that alignment with Legal / Procurement advice and false positive management would be important.

HTX Procurement Leader shared that the tool “really helps to provide a first-cut analysis of agreements/contracts and it’s fast” and suggested practical workflow enhancements such as Word report export and draft escalation emails for risks requiring internal escalation.

MOE CIO Team highlighted that the tool helps provide “the first cut of the potential risks involved in signing the EULA” and can “alert and provide guidance on the types of risks and severity of the risks”. MOE also identified a real operational gap in legal expertise within procurement / project teams.

DSTA Procurement Leader found that the prototype surfaced third-party / open-source component risks that procurement officers may not usually consider in manual review, and noted that such findings could prompt further technical assessment. DSTA also provided detailed feedback on improving clause referencing accuracy and expanding risk coverage.

Overall, stakeholders expressed interest in the direction of the tool as a first-pass informational aid that can support, but not replace, existing Legal / Procurement review processes. Their feedback has been used to refine the product roadmap, including improving traceability, adding confidence indicators, generating Word reports, and creating draft escalation emails.
# Solutioning
## Problem-Solution Fit
Deal Makers addresses the pain point by turning specialised contract review knowledge into a guided first-pass workflow. It helps officers identify common risks in ICT contracts, SaaS terms, EULAs, and pricing schedules; understand why they matter; and know what to escalate for further review.

By providing clause evidence, risk classification, explanations, consequences, and suggested next steps, the tool helps officers get up to speed faster and engage Legal, Procurement, technical teams, or approving authorities earlier. It supports existing review processes rather than replacing them.
## Functionality
1. Contract intake
User uploads ICT contract documents such as EULAs, SaaS terms, licensing agreements, order forms, pricing schedules, product terms, or vendor policies.
1. AI-assisted risk analysis using internal playbook
Deal Makers analyses the uploaded documents against a GovTech-developed playbook to identify common commercial, legal, operational, governance, licensing, data, and compliance risks.
1. Structured risk classification
Each detected issue is classified by severity, such as Critical / High / Medium, with confidence indicators and clause evidence so users can understand why the issue was flagged.
1. Plain-English risk explanation
For each issue, the tool explains:
  - what the clause means
  - why it matters in a Government context
  - possible consequences
  - what the officer should consider next
1. Guided next actions
The tool suggests whether the issue should be escalated internally, reviewed by Legal / Procurement / technical teams, accepted with conscious risk acceptance, or used as a negotiation point with the vendor.
1. Top risks summary
The tool provides a prioritised summary of key risks so users can quickly focus on the most important issues instead of reading the entire contract from scratch.
1. Contract risk coverage checklist
The tool shows which key risk areas were identified in the document and which areas were not detected, so users know what still requires human review.
1. Workflow outputs
Users can generate practical outputs such as:
  - a Word risk analysis report
  - draft escalation email to Legal
  - draft escalation email to management / approving authority
1. Human-in-the-loop review
The tool clearly positions its output as a first-pass informational review. Final assessment remains with the relevant officer, Legal, Procurement, technical team, or approving authority.
## User Experience
We made the experience seamless by keeping the workflow simple: upload contract documents, run first-pass risk analysis, review prioritised issues, and generate next-step outputs. The tool accepts common ICT contract documents such as EULAs, SaaS terms, licensing agreements, pricing schedules, and order forms.
Results are presented in a decision-friendly format, with top risks, severity classifications, clause evidence, plain-English explanations, consequences, and suggested next actions. Users can scan high-risk areas quickly or expand each issue for more detail. The tool also supports Word reports and draft escalation emails, helping officers move from review to action with minimal friction.
## User Validation
Users validated Deal Makers as a useful first-cut review tool for ICT contracts, SaaS agreements and EULAs. IMDA CIO found that it gives a “structured way to gather insights” and a “quick glance and appreciation of the risks”. HTX Procurement Leader shared that it “really helps to provide a first-cut analysis of agreements/contracts and it’s fast”. MOE ISM noted that it helps provide “the first cut of the potential risks involved in signing the EULA” and guidance on risk types and severity. DSTA Procurement Leader also observed that the tool surfaced third-party / open-source component risks which procurement officers may not usually consider in manual review.
Areas for improvement include improving page / clause reference accuracy, reducing false positives, expanding risk coverage to areas such as Liquidated Damages and Late Payment clauses, exporting reports in Word format, and generating draft escalation emails for Legal or management review. These have been incorporated into the product roadmap, while keeping final assessment with human reviewers.
# Impact & Next Steps
## Success Metrics
Utilisation rates by officers before a contract comes to Procurement/Legal for review – if users flag out their high-level alignments before a contract comes to Procurement/Legal for review, this indicates that the users are aware that there is a knowledge gap and the use of the tool facilitate their internal alignment.
## Expected Impact
Deal Makers can deliver immediate impact by reducing the time and effort needed for officers to make sense of ICT contracts before formal review. Instead of starting from a blank page, officers get a structured first-pass view of key risks, severity, clause evidence, consequences and recommended next steps.

This improves the quality of internal escalation, helps Legal and Procurement receive better-contextualised queries, and enables risks to be surfaced earlier in the procurement or contract management lifecycle. In the short term, the product can improve speed, consistency and confidence in ICT contract risk review, especially for officers who do not handle contracts regularly.

Over time, the tool can evolve into a reusable GovTech knowledge base of common ICT contract risks and standard positions, supporting more consistent contract assessment across teams and potentially across Government.
