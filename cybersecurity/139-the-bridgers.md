---
title: "The Bridgers - DocuHelp"
description: "A disconnect between risk intent and evidence interpretation weakens assurance - wasting up to 280 hrs/audit on misdirected effort."
sidebarTitle: "The Bridgers"
icon: "users"
---

# The Bridgers - DocuHelp

| Field | Value |
| --- | --- |
| Requested team | Bridgers |
| Judging group | Final Judging Group 3 |
| Scheduled time | 2:03pm |
| Team number | 139 |
| Category | Cybersecurity |
| Booth | 8B-11 |
| Project page | [https://build.tech.gov.sg/projects/2026/139](https://build.tech.gov.sg/projects/2026/139) |
| Product link | [https://gt-docuhelp-frontend-main.cio.sandbox.gov.sg/login](https://gt-docuhelp-frontend-main.cio.sandbox.gov.sg/login) |
| Team members | Anjana Balakrishnan From.cogn; Desmond Kwa; Gui An Lee; Li Shan Kua; Riven Ooi |
| Match status | normalized-the |

## Summary

A disconnect between risk intent and evidence interpretation weakens assurance - wasting up to 280 hrs/audit on misdirected effort.

## Full Write-Up

# Pitch Deck
DocuHelp_Final_Pitch_Deck.pptx (https://wjbbfxaztzhszi7i.public.blob.vercel-storage.com/collab-attachments/cmnwsvp92000w04lb4wbdkk9z/019e5cc2-0784-759d-8d9f-cb550ed45843-DocuHelp_Final_Pitch_Deck.pptx)
# Problem Statement
## Users
DocuHelp serves two primary user groups across Singapore’s public sector:
• Auditees across audited agencies — including IT officers, system owners, and security teams — who must continuously demonstrate their systems’ risk controls and respond to audit evidence requests.
•  ICT Auditors from CAT 4A and 4B vendors and agencies’ internal audit officers, including IT Audit Managers and junior ICT auditors who conduct the majority of fieldwork but often lack experience in clearly articulating requirements and identifying alternative evidence sources.
## Use Case
During the fieldwork phase of an ICT audit, auditors and agency IT teams must collaborate to validate risk controls against audit objectives. Auditors need to communicate specific evidence requirements clearly, while auditees must interpret these requests and submit evidence that proves their risk mitigations are adequate. This process requires alignment sessions, clarification rounds, and multiple submission cycles — all currently manual and error-prone.
## Pain Point
The root cause is a systemic lack of proactive clarity at the point of request. Evidence requests are issued without sufficient context on intent or acceptable evidence scope, and auditees have no structured way to understand requirements before they begin gathering evidence. Specifically:
•  Junior auditors frequently issue RFIs without surfacing the underlying audit objective, leaving auditees to guess what will be accepted.
•  There is no mechanism for auditees to proactively assess evidence sufficiency before submission, leading to reactive last-minute scrambles.
•  When primary evidence is unavailable, neither party has a structured way to identify mutually acceptable alternatives upfront, forcing multiple back-and-forth cycles.
•  Manual Excel-based tracking lacks integration with government data repositories (e.g. Government DCS), making it difficult to monitor outstanding items and plan submissions in advance.
## Consequence
Failing to bridge this gap has measurable impact on both audit quality and agency productivity:
•  The planned 8-week fieldwork timeline extends by 1–3 weeks.
•  The planned 2-week clarification period balloons to 3–6 weeks.
•  Audit engagements consume 80–280 additional hours (~10–35 days) per engagement in repeated submission-validation cycles.
•  Prolonged clarification strains working relationships between IT teams and auditors.
•  Time pressure can force acceptance of suboptimal evidence, compromising audit quality and the agency’s true risk visibility.
# User Research and Market Analysis
## User Research
The problem was validated through direct engagement with stakeholders from the audit ecosystem:
•  Interviews with practising ICT auditors and auditees from GovTech and public sector agencies confirmed that multiple rounds of clarification per engagement are the norm.
•  Junior auditors acknowledged difficulty articulating the intent behind evidence requests; auditees confirmed they regularly struggle to identify what would be “good enough” evidence.
•  Key insight: Auditees need structured, upfront guidance on what is required and what alternatives exist — not just a chatbot to query after they get stuck.
## De-risking
• Adoption risk: Auditors may resist changing Excel-based workflows and still rely on DCS repository for RFI submissions. Mitigation: DocuHelp generates RFI requests (primary and alternative evidence) directly from uploaded audit work programme documents, using AI to explain the audit intent, checking the RFIs against the requested evidence to ensure  completeness, relevance, and sufficiency before submission.
• Data sensitivity risk: Audit evidence may include sensitive government information. Mitigation: Platform is designed for deployment within government infrastructure; all data stays within agency-controlled environments. Also, users are required to acknowledge (as a form of declaration) uploaded files do not exceed Restricted / Sensitive Normal, and this trail will be saved to database for record purposes.
•  AI accuracy risk: Auto-generated RFIs may miss critical objectives. Mitigation: Implemented AI validation programme with DocuHelp to check the output. Auditors will also have to review and edit all AI-generated RFIs before sharing; human oversight is built into the workflow.
## Stakeholder Buy-in
GovTech CDA, who conducts central ICT audits on agencies using CAT 4A vendors, has validated the problem statement and solution approach. On the auditee side, we engaged MCCY and GovTech CSG — both of whom work directly with auditors during audit engagements — and they expressed strong interest. Additionally, GovTech DTG have also expressed interest in DocuHelp as a tool to collect and validate SSP compliance.
# Solutioning
## Problem-Solution Fit
DocuHelp directly addresses the proactive clarity gap by:
•  Auto-generating structured, intent-rich RFIs from audit work programs: multi-agent AI analyses audit objectives, risks, controls, and test procedures to produce 20–70 structured evidence requests, each articulating why the evidence is needed (control objective) and what is acceptable (primary and alternative evidence). Auditees know exactly what to provide before they begin.
• Providing an AI Evidence Pre-check that auditees run before submission: uploaded files are matched against the evidence checklist item-by-item, flagging gaps ("partially covered", "not covered") with actionable suggestions, catching insufficiencies early rather than after auditor rejection.
• Surfacing alternative evidence and compensating controls proactively: every RFI item includes fallback options when primary evidence is unavailable, eliminating guesswork and reducing back-and-forth.
• Replacing manual Excel tracking with a centralised, role-based portal: auditors, auditees, and internal
reviewers each have real-time dashboards with status breakdowns, progress bars, deadline awareness, and submission versioning (v1, v2, v3…).
• Supporting internal clearance workflows: organisations that require evidence to be reviewed internally (e.g. by a CISO) before release to auditors can configure mandatory or optional clearance gates, ensuring compliance without slowing down teams that don't need it.
## Functionality
Auditor Flow:
• Creates a new audit engagement, sets the audit period, and uploads one or more Work Programmes (PDF/Word/Excel).
• Labels each document with an audit theme (e.g. "Access Controls", "Change Management") for organised RFI grouping.
• Clicks "Generate RFI"— multi-agent AI processes documents in parallel (up to 4 simultaneously), analysing audit objectives, risks, and expected controls to auto-generate structured evidence requests. Each item includes a risk statement, control description, test type (design or operating effectiveness), control objective, and both primary and alternative evidence requirements. Progress is tracked in real time.
• Reviews, edits, adds, or removes RFI items. Can manually create additional items where needed.
• Shares the RFI with auditees via email — accounts are auto-provisioned with a one-time setup link. Can grant access to multiple auditees.
• Sets submission deadlines and can lock/unlock the RFI to control when evidence can be submitted.
• Optionally configuresinternal clearance: designates reviewers (e.g. CISO) and sets enforcement mode (mandatory — all evidence must be cleared; or optional — officers choose per item).
• Monitors submissions via a dashboard showing a review queue, deadline alerts, AI triage summary (sufficient vs. insufficient), and recent activity.
• Reviews submitted evidence: accepts, requests revision with structured feedback, or reopens previously accepted items — all with full version history.
Auditee (Officer) Flow:
• Receives portal access via email; sets up account with one click.
• Views all RFI items grouped by audit category, with full context: why the evidence is needed (control objective), what to provide (primary evidence), and what alternatives are acceptable— all visible upfront before starting.
• Acknowledges data classification requirements (Restricted / Sensitive Normal ceiling) before uploading.
• Uploads evidence files or links existing files already uploaded against other items in the same RFI — avoiding duplicate uploads.
• AI automatically pre-checks uploaded evidence against the checklist, showing item-by-item coverage status (covered / partial / not covered) with suggestions.
• Uses the AI chat assistant to clarify uncertainties and get context-aware guidance on what would satisfy the request.
• Adds clarification notes visible to both parties for coordination.
• Submits evidence for auditor review — or, if internal clearance is configured, routes for internal clearance first.
• If revision is requested: reviews auditor feedback, updates evidence, and resubmits as a new version.
• Can share access with colleagues who can also respond to evidence requests.
Internal Clearance Reviewer Flow:
• Receives designation as a clearance reviewer for an RFI.
• Views pending clearance requests on their dashboard — each showing the requester, items, attached files, and any notes.
• Reviews the evidence and either approves (evidence is auto-submitted to the auditor) or rejects with a comment (item returns to in-progress for the officer to address).
• Maintains a decision history for audit trail purposes.
## User Experience
• Zero-friction onboarding: auditors upload existing work programme documents as-is (no reformatting);
auditees are auto-provisioned with accounts — no manual registration or IT involvement needed.
• Proactive clarity over reactive chasing: every RFI item displays its control objective ("Why we need this"), primary evidence list ("What to provide"), and alternative evidence — auditees can plan their response before starting, not after a rejection.
• AI as a safety net, not a gatekeeper: the pre-check runs automatically after each upload, giving immediate
feedback. Auditees self-correct before submission; auditors see an AI triage summary to prioritise their review queue.
• Evidence reuse across items: officers can link files already uploaded against other RFI items, eliminating redundant uploads when the same document satisfies multiple requests.
• Structured submission versioning: every submission is captured as a snapshot (v1, v2, v3…) with the exact files at that point in time, auditor feedback, and timestamps — providing a clear audit trail without manual tracking.
• Flexible internal governance: the clearance workflow is entirely opt-in and zero-friction when not configured. Organisations that need internal sign-off get mandatory or optional clearance gates; those that don't see no additional UI or steps.
• Real-time visibility: both auditors and auditees have role-appropriate dashboards with progress bars, status breakdowns, deadline indicators, and activity feeds — replacing the "where are we?" emails.
• Context-aware AI chat: the assistant answers questions specific to each evidence request in plain language, suggesting concrete documents or actions rather than generic guidance.
## User Validation
DocuHelp was validated through hands-on testing with practising IT auditors and auditee officers from government agencies, with feedback collected iteratively and incorporated into the product in real time.

What worked well:
• AI-generated RFIs were immediately recognised as high-value. Auditors noted that the multi-agent approach produced structured, audit-ready evidence requests that closely mirrored what they would have written manually — but in minutes rather than days. The inclusion of control objectives, risk statements, and both primary and alternative evidence per item was cited as the clearest differentiator from existing Excel-based workflows.
• Auditees understood what was expected of them — before starting. Officers consistently reported that
seeing the "Why we need this" (control objective) and "What to provide" (evidence checklist) upfront eliminated the guesswork they typically experience. One tester described it as "the first time I didn't have to chase the auditor to clarify what they actually wanted."
• The AI pre-check reduced anxiety around submission. Auditees valued the immediate, item-by-item coverage feedback after uploading files. Knowing whether evidence was "covered", "partially covered", or "not covered" before the auditor reviewed it gave officers confidence to submit — or to address gaps proactively rather than waiting for rejection.
• Auto-provisioned accounts removed an adoption barrier. Auditees received a setup link, set a password, and were inside the portal within a minute. Testers contrasted this with the typical onboarding friction of enterprise tools that require IT involvement or separate registration workflows.
What required improvement (and how we addressed it):
• Evidence descriptions needed to be more prominent. Early testers missed the primary and alternative evidence lists because they blended into the item detail. We redesigned the layout with numbered evidence checklists, colour-coded sections (green for primary, amber for alternatives), and a prominent blue info banner explaining what the AI pre-check does — making requirements impossible to overlook.
• AI-generated date qualifiers on evidence items caused confusion. The AI initially appended date suffixes like "(current as at 2026-03-31)" to design evidence items, which is incorrect — design tests assess a point-in-time control, not a period. We implemented a two-pronged fix: a prompt-level rule prohibiting date qualifiers on design items, and a programmatic regex strip as a safety net. Operating effectiveness items now use the standard phrase "for the period under review (refer to sample size per sampling guide)" as auditors expected.
• Same document produced slightly different RFI counts across regenerations. Auditors flagged that regenerating from the same work programme sometimes yielded 40 items, sometimes 41. This non-determinism undermined trust in the AI output. We resolved it by setting the AI temperature to 0, producing consistent, reproducible results.
• Time estimates during generation were inaccurate. The initial estimate of "under 1 minute" for multi-document processing proved misleading when generation actually took 1–2 minutes. We replaced it with a batch-aware calculation that accounts for parallel processing (4 documents at a time), giving auditors a realistic expectation.
• Internal clearance was a missing workflow for government agencies. Several testers from agencies with information security requirements pointed out that officers cannot release evidence directly to external auditors — it must first be reviewed internally (e.g. by a CISO or designated approver). This was not in the original design. We built a full internal clearance workflow with two enforcement modes: mandatory (all items must be cleared) and optional (officers choose per item). The workflow adds zero friction when not configured — organisations that don't need it see no additional steps.
•  Submission controls needed more granularity. Auditors wanted the ability to lock submissions manually (not just via deadline) and for auditees to see the lock/open status clearly. We added manual
lock/unlock controls and a visible status indicator on the auditee dashboard, so officers always know whether submissions are open.
• Classification acknowledgement wording went through several iterations. The initial phrasing was unclear about what the auditee was confirming. After multiple rounds of feedback, we settled on explicit language: "I confirm that the files I am uploading are classified Restricted / Sensitive Normal or below. I understand that Confidential or Sensitive High documents must not be uploaded to this system."— with a persistent green confirmation once acknowledged.
•  The submit button should gate on AI completion. Testers observed that officers could click "Submit" or
"Route for Internal Clearance" while the AI pre-check was still running, potentially bypassing the safety net. We disabled action buttons until the AI evaluation completes and displays its results.
Key takeaway: The core value proposition — proactive clarity through AI-generated, intent-rich RFIs validated strongly from the first test. The majority of improvement feedback centred on edge cases in AI output quality, workflow completeness for government contexts, and UI clarity — all of which were addressed iteratively without changing the fundamental product direction.
# Impact & Next Steps
## Success Metrics
North Star Metric: Reduction in submission-validation cycles per RFI item (target: from an average of 3+ cycles down to 1–2 cycles).
Supporting metrics:
•  Total hours saved per audit engagement (target: reduce by 80–280 hours per engagement).
•  Fieldwork timeline adherence (target: engagements completed within the planned 8-week window).
•  First-submission acceptance rate (target: >70% of RFI items accepted on first submission).
## Expected Impact
Short Term (0–6 months):
•  Pilot with 2–3 audit engagements involving GovTech auditors and agency auditees.
•  Target: 50% reduction in repeated submission cycles; fieldwork stays within the planned 8-week
timeline.
Medium Term (6–18 months):
•  Expand to CAT 4A/4B audit vendors and additional public sector agencies.
•  Integrate with Government DCS for automated evidence retrieval, further reducing auditee effort.
Long Term (18+ months):
•  Establish DocuHelp as the standard evidence management platform across Singapore’s public sector ICT audit ecosystem.
•  Build a knowledge base of accepted evidence patterns to continuously improve AI suggestions and reduce
audit cycle times.
