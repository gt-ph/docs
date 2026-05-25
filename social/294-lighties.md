---
title: "Lighties - FieldNote"
description: "Mobile-first, context booking solution that allows caseworkers to capture high-fidelity insights in real time."
sidebarTitle: "Lighties"
icon: "users"
---

# Lighties - FieldNote

| Field | Value |
| --- | --- |
| Requested team | Lighties |
| Judging group | Final Judging Group 1 |
| Scheduled time | 2:56pm |
| Team number | 294 |
| Category | Social |
| Booth | 8E-04 |
| Project page | [https://build.tech.gov.sg/projects/2026/294](https://build.tech.gov.sg/projects/2026/294) |
| Product link | [https://fieldnote-v1.app.tc1.airbase.sg/](https://fieldnote-v1.app.tc1.airbase.sg/) |
| Team members | Alicia Tan From.accenture; Fugene Choy; Jiayi Lu From.businessedge; Nuno Jonet; Victoria Koo |

## Summary

Mobile-first, context booking solution that allows caseworkers to capture high-fidelity insights in real time.

## Full Write-Up

# Problem Statement
## Users
The primary users are MSF PSV Child Protection Case Workers. Each officer typically handles a caseload of 20 to 30 clients per month. These individuals operate in high-stakes, high-empathy environments where accuracy and speed of information are critical for child safety. They conduct home visits and in-person engagements with at-risk children and families.
## Use Case
Child Protection case workers at MSF are responsible for supporting vulnerable families and clients in the field. During client interactions, they must capture detailed observations, take notes, and update their supervisors on case developments. Officers gathered information through conversational formats, including voice notes, mobile messages, and handwritten observations.
The official Case Management System (CMS) is the central repository for all case-related data. Officers will document all information in the CMS. As a desktop-only platform, it therefore lags the case notes by days to weeks on any given open case.
## Pain Point
1. Current tools not built for field use: Vital context is lost as tools are desktop-first, making real-time note-taking of detailed observations challenging.
1. Memory recall and time lag: Mental Fatigue and documentation lag means delay of timely interventions.
1. Scattered and Fragmented data : 2-3 extra hours piecing together notes scattered across handwritten notes, chats and voice memos.
## Consequence
This directly undermines the accuracy, timeliness, and quality of safeguarding decisions, as officers spend significant time manually reconstructing notes, extracting actions, and updating records across fragmented systems. The resulting administrative overhead slows the critical “Time to Safety” response window and reduces the time, attention, and quality of care officers can provide to vulnerable families in need.
# User Research and Market Analysis
## User Research
Below are the key user research methods we adopted to validate this solution.
Ultimately, the research highlights that while caseworkers are passionate about the work they do, the "vicious cycle" of manual tracking, where frontline officers resort to personal OneNote, mobile apps, WhatsApp, and voice recording to capture their field visits, is stored on their local personal devices. If these do get uploaded to a central system, there is always a lag because of how cumbersome and non-intuitive they are to use. The absence of a quick ability to share live updates on a case produces a Systemic Risk.
[table block omitted in flat markdown; see narrativeBlocks in JSON]
## De-risking
The key assumption is that case workers might not use yet another tool.
We have created an AI-powered synthesis of notes that quickly tells us the key issues and decisions that need to be made. These vital ground-level signals (captured on personal devices) now become visible instead of remaining siloed from central monitoring systems.
This technical and administrative friction, which transforms administrative delays into a profound systemic risk, now enables agencies to identify escalating patterns of harm before they reach a crisis point because of the added real-time visibility.
We are closing the gap between capturing field notes and sharing them immediately for key decision-making.
## Stakeholder Buy-in
We have reached out to Protective Services (PSV) Officers at MSF and to the day-to-day operations users. They expressed keen interest in piloting this.
# Solutioning
[image](https://wjbbfxaztzhszi7i.public.blob.vercel-storage.com/collab-media/cmny8xv2i000304jpn7qyywf3/019e59cc-6f58-7409-9b12-cd4703e42a69-image.png)
## Problem-Solution Fit
Mobile first Context Capture
Accessible, real time context tagging captured in the moment, on the go, enabled by Tap to flag feature.
AI-powered, Domain- shaped synthesised notes
Summaries are structured using pre-populated templates with human in the loop review.
Workflow integrated sharing and exportability
Fits into current workflow using whatsapp and email for faster supervisor visibility and decision making.
## Functionality
### 1. Tap-to-Flag
Instantly bookmark crucial moments in the transcription without breaking eye contact or flow.
Outcome: Minimised delays between field interactions and documentation.
### 2. Domain-Shaped Structured Synthesis
Pre-populated templates are tailored to specific fields of work;  synthesised into key categories,  issues, and actions. The caseworker retains full control to review and edit, with quick reference of bookmarked transcriptions, all while on the go.
Outcome: Minimised delays between field interactions and documentation.
### 3. Share & export to existing channels
Safeguarding decisions require absolute accuracy and rapid communication. Insights can be immediately exported to WhatsApp or email, shortening time it takes to share progress and decisions with supervisors.
Outcome: Timely safeguarding decisions made.
### 4. Supports multi-languages
Understands Southeast Asian languages and code-switching, including Singlish, for accurate real-world capture.
Outcome: Capture confidently without worrying about accents, dialects, or mixed language being missed
### 5. Tailored roles and note templates
Create role-specific templates and let AI generate structured summaries based on the defined format.
Outcome: More tailored outputs with less need for manual editing
### 6. Chat with case notes using natural-language
Instantly retrieve specific case details by asking questions in natural language; no need to dig through long transcripts.
Outcome: Quick access to key context without manual searching
## User Experience
1. One-tap capture. Officers start a note and start talking - no form, no dropdown, no case-status selection between opening the app and the first sentence. Real-time transcription runs while the conversation continues. This removes the friction that currently pushes officers into generic notes apps: anything that asks them to categorise before they've finished thinking.
1. Quick, scannable summary. Every AI summary uses the same three-part structure: Key points, flags and issues, and key actions. Tap-to-flag during capture lets the officer mark important moments in the conversation, and the AI weights flagged segments in the summary.
1. Officer in the loop, AI on the side. The AI summarises and answers single-note queries, but never auto-pushes to the supervisor and never proposes next-step decisions. The officer reviews, edits, and shares.
## User Validation
- The core functionality covers essential caseworker workflows, including capturing visits, reviewing AI-generated notes, filing notes under cases, and sharing outputs.
- The integration with the Web Speech API allows for hands-free recording during home visits.
- The product provides multiple sharing options, including WhatsApp and Email.
# Impact & Next Steps
### Integration to MSF Caseworker Ecosystem
1. MSF CMS Integration: Seamlessly integrate with Case Central CMS to streamline data flow.
1. Deployment to GCC environment: Ensure proper security controls are built in.
1. Scale to other MSF user groups: Future-proofed to scale effectively to vulnerable adult cases.
### Scaling Opportunities
Identified government targets with use cases tailored to each agency:
Inspection and compliance (on-site visits)
- ECDA - Regulatory site visits
- NEA - Hawker inspection/cleanliness checks
- MTI - Licensing inspections
Frontline field operations
- SPF - Law enforcement
- ICA - Immigration and related work
These are roles in government requiring field operations, in-person interactions, and documentation for evidence.
## Northstar Metrics
1. Reduce documentation time: Caseworkers save 1 working day (8-12 hrs/week) and reduce burnout.
1. Reduce data gap: Minimising note-upload to CMS, ensuring team continuity and case follow-throughs.
1. Faster intervention for at-risk children: Timely case developments directly improve safety outcomes for children.
#### Pitch Deck
[file]
[file](Lighties Pitch Deck_Final.pdf)
[file](https://docs.google.com/presentation/d/1V9E-OkYVjjJmBCLjLg0ZXyhqxFLtQhRx8zP6yhMhIYk/edit?slide=id.g3e9ebba1a81_3_80#slide=id.g3e9ebba1a81_3_80)
