---
title: "Fin Automation - Finance Automation Tools"
description: "Central hub for government finance & procurement teams to find, use and share automation tools - no more starting from scratch."
sidebarTitle: "Fin Automation"
icon: "users"
---

# Fin Automation - Finance Automation Tools

| Field | Value |
| --- | --- |
| Requested team | Fin Automation |
| Judging group | Final Judging Group 1 |
| Scheduled time | 2:46pm |
| Team number | 135 |
| Category | Economy & Finance |
| Booth | 10F-12 |
| Project page | [https://build.tech.gov.sg/projects/2026/135](https://build.tech.gov.sg/projects/2026/135) |
| Product link | [https://fin-automation-tools2.cio.sandbox.gov.sg](https://fin-automation-tools2.cio.sandbox.gov.sg) |
| Team members | Darren Kam; Kaden Koh; Khong Beng Kang; Lisa Lim From.scientec; Yihua Luo |

## Summary

Central hub for government finance & procurement teams to find, use and share automation tools - no more starting from scratch.

## Full Write-Up

Slide deck: https://canva.link/hw3z230rpk9aaoj
# Problem Statement
## Users
Finance and procurement officers across government agencies (such as the people who handle month-end closing, year-end accruals, purchase order management, and other recurring financial tasks). Also for the in-house developers and "vibe coders" who build the tools these teams rely on.
## Use Case
- Every month, government finance and procurement teams spend large amounts of time on repetitive, manual work — processing accruals, reclassifying journal entries, and retagging hundreds of purchase orders when agencies restructure. This work is time-pressured, error-prone, and happens at scale across dozens of agencies.
- Teams have tried to solve this with automation: expensive RPA bots (~$20,000 each with maintenance contracts), Excel macros, Python scripts, and recently, AI-assisted "vibe coding." But every team builds alone. There is no shared place to discover what others have already built, so agencies unknowingly solve the same problems over and over again.
- Worse still, when the person who built a tool leaves the agency, the tool disappears with them. There is no way to preserve that work or pass it on.
## Pain Point
- No centralised discovery layer: There is no "app store" for government finance tools. Agency A builds a PO retagging tool. Agency B, which is unaware of what Agency A has done, spends weeks building the exact same thing.
- Too hard to share: Even when someone builds a useful tool, turning it into something colleagues can actually use (with proper login, security, and a simple interface) typically takes weeks of extra work. Most tools never make that leap, and instead stay as private scripts, invisible to everyone else.
- Fragile and expensive: RPA bots are costly and require dedicated licences just to run. Excel macros break due to updates and logic changes. Scripts stop working when their creator rotates out.
- High error rates: According to a 2025 analysis, manual journal processing has been found to have error rates as high as 49%, which is nearly 1 in 2 entries requiring correction or rework during critical close periods.
[image](https://wjbbfxaztzhszi7i.public.blob.vercel-storage.com/collab-media/cmnwsteai001z04l44exg45hn/019e05cd-2223-758a-8df9-b7b2e9ee0fcf-image.png)
## Consequence
•	Duplicated build effort across WOG: 
Without a central discovery layer, agencies independently solve the same problems. If just five agencies each replicate three common automations at four weeks of effort each, that is 60 person-weeks of wasted work annually — a conservative estimate.

•	Continued and unnecessary vendor dependency: 
Large-scale events like organisational restructuring currently require external consultants to perform PO retagging at significant cost. This dependency is entirely avoidable with the right internal tooling, and leaving it unsolved means that cost recurs every time a reorg happens.

•	Over reliance on AGD / PSD as a central consulting party: 
Without a scalable automation platform, AGD / PSD remain a bottleneck for implementing and supporting agency level automation, increasing their operational burden and limiting their ability to focus on higher value, cross government initiatives.

•	Operational fragility due to platform and environment constraints:
Macro  and script based tools are sensitive to operating system and platform limitations (e.g. unsupported macro functions across environments). Recent incidents have shown that such failures can surface at critical periods, triggering last minute fixes, uncertainty among operational teams, and pressure on central teams to expedite releases — despite minimal end user tolerance for disruption during close cycles.

•	Operational and audit risk at financial close: 
Manual accrual entries and reclass processing during high-pressure close periods introduce material error risk into financial statements, with downstream consequences for audit integrity and reporting accuracy.

•	Silent loss of institutional knowledge: 
Macro-based and script-based tools are tied to the individuals who built them. As officers rotate or leave, these tools break or disappear entirely — automation capital that took significant effort to build evaporates with no recovery path.

•	Stalled automation adoption: 
Without a low-friction path from script to production-ready tool, capable developers deprioritise building. The two-week productionisation burden acts as a tax on every automation initiative, meaning many potential efficiency gains across WOG are never realised.
# User Research and Market Analysis
## User Research
1) Interviews
- We interviewed finance and procurement stakeholders across GovTech to understand how much time is lost to manual tasks, how fragile existing automation tools really are, and whether teams would actually use a shared platform if one existed.
- Key insights:
  - Interviews with Procurement Buyers identified mass Change Order processing as a critical manual bottleneck, currently requiring 35 minutes of effort per Purchase Order (PO). By transitioning from manual workflows to our centralized platform, we project a reduction in processing to just 10 minutes per PO—representing a >70% improvement in operational efficiency.
2) Live Trial
- Rather than wait for validation, we ran a real-world trial with GovTech's Finance team, who have been using the platform in their actual daily work since March 2026 - including for Year-End accruals closing. The Procurement team has since onboarded their tools onto the platform as well.
- Since March, the platform has seen more than 594 files processed with a total of 2.2 million rows of data.
- One notable example from year-end closing was the EIB automation tool, which transforms simplified Excel files into Workday-ready EIB formatted templates, handling data transformation and lookups internally. This tool was used 221 times, processing 290 files in total. A survey of users found that it has greatly reduced file rejection rates, from over 30% down to just 1-5%. Compared to the previous Excel macros approach, users rated the experience as significantly better, describing the process as smoother and less frustrating.
- Early feedback from finance officers highlights two things: the drag-and-drop interface removes the need to run local Python scripts or Excel setups, and having a single place to find tools means they no longer have to ask around or build solutions from scratch.
Is there appetite to scale?
- Finance and procurement processes are broadly similar across government agencies, since a tool built for GovTech's month-end close can, in principle, be used by any other agency.
## De-risking
[table block omitted in flat markdown; see narrativeBlocks in JSON]
## Stakeholder Buy-in
We are in early conversations to get AGD and PSD to evaluate the platform for wider adoption.
# Solutioning
## Problem-Solution Fit
The idea in one sentence:Finance Automation Tools is a shared platform, think of it as a "government app store" for finance automation, where teams can find tools others have built, use them instantly via a clean web interface, and contribute their own.
## Functionality
- How it works:
- Part 1 — Tools Library A searchable catalogue of ~15 finance and procurement automation tools, organised by use case. Users simply drag and drop their files in and get their output, with no Python, no Excel setup, no local dependencies. Every tool on the platform comes with built-in authentication, access control, audit logs, and a proper UI — all handled automatically by the platform.
- For tool builders, this means they can focus entirely on the logic of their automation. The platform takes care of the rest, eliminating the weeks of extra work that normally prevent useful scripts from ever becoming usable tools.
- Part 2 — Community Forum A space where finance and procurement officers can post problems they're struggling with, propose solutions, or request tools. This turns individual pain points into community knowledge, and creates a pipeline for future tools to be built.
## User Experience
- What makes this different from what exists today:
[table block omitted in flat markdown; see narrativeBlocks in JSON]
## User Validation
- As mentioned above during the live trial, users have rated the experience as significantly better, describing the process as smoother and less frustrating. They have also feedbacked that the drag-and-drop interface removes the need to run local Python scripts or Excel setups, and having a single place to find tools means they no longer have to ask around or build solutions from scratch.
# Impact & Next Steps
## Success Metrics
- Hours saved: Total person-hours redirected from manual transactional work to higher-value tasks
- Reuse rate: Number of times a tool built by one team is used by another team or agency
## Expected Impact
- Short Term: Reduce wasted effort on duplicated builds across government; decrease vendor dependency for reorganization tasks.
- Long Term: Much like GitHub changed how software developers work by letting them build on each other's code, Finance Automation Tools aims to ensure that every automation built in government compounds in value — rather than disappearing into a silo when someone changes jobs. The goal is a self-sustaining ecosystem of reusable tools that makes every agency smarter over time.
