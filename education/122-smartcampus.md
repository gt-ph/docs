---
title: "SmartCampus - Smart Campus AI"
description: "AI-powered school investigation platform that finds incidents, identifies persons of interest, and compiles evidence in minutes."
sidebarTitle: "SmartCampus"
icon: "users"
---

# SmartCampus - Smart Campus AI

| Field | Value |
| --- | --- |
| Requested team | Smart Campus |
| Judging group | Final Judging Group 4 |
| Scheduled time | 1:30pm |
| Team number | 122 |
| Category | Education |
| Booth | 9E-01 |
| Project page | [https://build.tech.gov.sg/projects/2026/122](https://build.tech.gov.sg/projects/2026/122) |
| Team members | Jun Wei Ng From.tp; Kanashima Hatsumi; Luke Goh; Rahmuna Abdul Samad; Sone Kyaw Pye |

## Summary

AI-powered school investigation platform that finds incidents, identifies persons of interest, and compiles evidence in minutes.

## Full Write-Up

# Problem Statement
## Users
School Leaders and Discipline Teams across Singapore's 147 secondary and 182 primary schools (329 schools in total), with downstream impact on the student population they serve.
## Use Case
When an incident is reported, discipline staff must reconstruct what happened, typically by estimating the time and location, then scrubbing CCTV footage to identify the parties involved and the sequence of events. They do this to verify reports, identify perpetrators and witnesses, and compile evidence for follow-up action.
## Pain Point
The investigation process is entirely manual. Each physical incident takes on average 1.5 staff members between 45–60 minutes each, with most of that time spent estimating time/location windows and manually scrubbing footage. Because investigation capacity is constrained by limited staff bandwidth, discipline teams are only able to focus on high-confidence cases and cannot afford to pursue weaker signals or emerging leads during an investigation. As a result, early indicators of repeated or escalating bullying are often missed, simply because there is insufficient time to explore them.
## Consequence
Schools handle on average 3–4 physical incidents per week. At current rates, this diverts an estimated 38,164 staff-hours annually across Singapore schools (low estimate; midpoint ~52,640 hours) away from higher-value educational work. More critically, the bottleneck reinforces a detection gap: MOE data records 3 cases per 1,000 primary students and 8 per 1,000 secondary students, while a 2025 CNA survey found 30% of students reported bullying experiences meaning only 0.3–0.8% of actual incidents reach official records. Without effective and timely ways to detect bullying, schools remain reliant on reactive responses, missing opportunities for early intervention and leaving parliamentary concerns over schools’ role in preventing bullying unaddressed.
# User Research and Market Analysis
## User Research
The team conducted user interviews with discipline masters and vice-principals across 8 schools to validate the problem space.
The signal so far has been consistent: every interviewee independently confirmed that manually scrubbing CCTV footage is one of the most painful parts of their investigation workflow, validating both the existence and the severity of the bottleneck.
## De-risking
[table block omitted in flat markdown; see narrativeBlocks in JSON]
## Stakeholder Buy-in
We have engaged School Superintendent Janis, Zonal Directors for Schools for the West and South and Deputy Director-General of Education (Schools) to secure buy-in on the problem framing and proposed direction.
# Solutioning
## Problem-Solution Fit
The tool directly removes the most time-consuming steps in the current investigation workflow. Instead of estimating windows and scrubbing footage manually, staff can query the system for an event of interest, object of interest or person of interest within a defined time and location window, and have relevant events surfaced automatically. This collapses a 60 minutes task into 10 minutes, freeing capacity to follow secondary leads, the indirect path to earlier detection of sustained bullying.
## Functionality
  - Footage ingestion into a searchable index
  - Person-of-interest search across defined time and location windows
  - Event surfacing for incidents of concern (e.g. physical fights, theft), without manual scrubbing
## User Experience
Because this is a new technology in schools and discipline teams have understandable concerns about handling footage containing student faces, we deliberately designed the initial experience to be non-invasive and school-controlled: rather than integrating directly with school CCTV systems, discipline teams upload the relevant footage themselves into the tool. This keeps schools firmly in control of what data enters the system and when, lowering the trust barrier for first-time adoption and aligning with data and AI governance principles.
Once footage is uploaded, staff can search for a person of interest, review surfaced events, and export an evidence package, without ever needing to scrub raw footage manually. As trust is established and the governance framework matures, deeper integration can be considered in future phases.
## User Validation
Have yet to conduct user validation at this point in time. Will add it in once done.
# Impact & Next Steps
## Success Metrics
Hours reclaimed per school per week through faster investigations
## Expected Impact
Short term (Phase 1):
- ~6× faster investigations (60 → 10 minutes per case)
- ~4 staff-hours returned per school per week (midpoint estimate; range 2.9–5.3 hours)
- ~52,640 staff-hours returned annually across Singapore schools at midpoint (range 38,164–69,748) — roughly 72 months of staff time redirected to higher-value educational work each year
Medium term:
- Lower investigation friction enables staff to pursue secondary leads that previously went uninvestigated, increasing the likelihood of uncovering sustained bullying earlier
- Establishes the technical foundation (footage ingestion, search, person/event indexing) and governance framework (access controls, retention policy) required for any future proactive capability
Long term:
- Pattern-based flagging — for example, identifying students recurring across multiple incidents — to shift schools from reactive to proactive detection
- Phase 2 scope, feasibility, and privacy framework to be assessed based on Phase 1 outcomes
- Direct contribution to closing the gap between the 0.3–0.8% recorded incidence rate and the 30% student-reported experience rate, addressing parliamentary concern over schools' capacity to detect bullying earlier
