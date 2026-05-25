---
title: "SportsGenie - SportsAssist"
description: "Manual tracking by 700+ coaches for 50,000 participants yearly creates silos, wasting time and blocking talent insights."
sidebarTitle: "SportsGenie"
icon: "users"
---

# SportsGenie - SportsAssist

| Field | Value |
| --- | --- |
| Requested team | Sports' Genie |
| Judging group | Final Judging Group 1 |
| Scheduled time | 1:53pm |
| Team number | 105 |
| Category | Communications and Engagement |
| Booth | 1E-15 |
| Project page | [https://build.tech.gov.sg/projects/2026/105](https://build.tech.gov.sg/projects/2026/105) |
| Product link | [https://staging.gvt-build26-sportsassist.stg.paas.sandbox.gov.sg/](https://staging.gvt-build26-sportsassist.stg.paas.sandbox.gov.sg/) |
| Team members | Ana Ng; Esther Ng; Howard Liu; Jin Chin Quek; Junias Lim |

## Summary

Manual tracking by 700+ coaches for 50,000 participants yearly creates silos, wasting time and blocking talent insights.

## Full Write-Up

# Problem Statement
## Users
700+ coaches, 25 admin staff, ~50,000 non-unique participants, and ~100,000 parents/guardians across 10 sports annually
## Use Case
What coaches are trying to do:
- Record observations of each participant's performance in real time
- Convert raw notes into structured, progress report
- Share these reports with diverse parent groups who expect clear, personalized updates
- Submit consolidated reports to ActiveSG Academies & Clubs (A&C)

Coach's Tasks:
- Observe and assess participant on both sport-specific skills (e.g. agility, accuracy) and behaviours (e.g. teamwork, discipline)
- Translate assessment scores into the progress report format
- Liaise with parents with different expectations (e.g., detail-oriented vs. high-level summary)
- Share reports timely with parents and ActiveSG A&C

Where: Assessments are done on-field during sessions; translation of scores done post-session
 
When: 3-5 sessions before the season ends
## Pain Point
Absence of a Systematic Progress Tracking Framework   
Coaches lack a structured, user‑friendly system to consistently monitor and document participant progress across sport‑specific indicators. Without this, improvement trends, development patterns, and comprehensive records cannot be effectively maintained—leading to inefficiency, lost insights, and uneven service delivery.

Reliance on Manual, Siloed Processes
ActiveSG A&C relies heavily on manual and siloed processes. There is no centralized digital platform or standardized framework that integrates performance tracking across academies. As a result, coaches are forced to improvise with fragmented tools (spreadsheets, paper notes, ad‑hoc reports), which creates inconsistency, drains time, and prevents scalable, reliable progress monitoring.
## Consequence
Administrative Overload: 700+ coaches face hundreds of manual records each season, leading to data entry errors

Lost Insights: With records scattered across silos, identifying trends or development patterns is tedious and time-consuming.

Scalability Risk: Without consolidated data, ActiveSG A&C cannot evaluate youth talent potential effectively.

Time Savings: Estimated ~480,000 minutes per year could be saved across 10 sports for coaches

Strategic Impact: Without digitisation, SportSG risks missing its mission to engage youth in sports and groom national talent pipelines.
# User Research and Market Analysis
## User Research
What user research methods did you adopt to validate that this solution is needed and what were the key insights from real users?
## Method 1: Stakeholder Interviews & Workshops
12 sessions total — 10 workshops and 2 on-site interviews across basketball and water polo, engaging head coaches, assistant coaches, sports administrators, and parents.
These sessions helped us map end-to-end processes across basketball, water polo, and canoeing, surface operational pain points, and test our prototype directly with users.
[table block omitted in flat markdown; see narrativeBlocks in JSON]
## Method 2: Parent Survey
134 responses collected to understand parents' existing experiences and appetite for progress reports.
[table block omitted in flat markdown; see narrativeBlocks in JSON]
## What the Research Told Us to Build
The interviews and survey converged on three clear design imperatives:
1. Automate the assessment-to-report pipeline so that every participant gets a report, every season, without manual effort from coaches.
1. Personalise feedback using AI so that comments and remarks are meaningful and developmental, not generic.
1. zDeliver flexibly via portal and WhatsApp/email so that parents receive reports in the channel they trust.
## De-risking
What market risks are there and how did you mitigate them?
[table block omitted in flat markdown; see narrativeBlocks in JSON]
## Stakeholder Buy-in
Which agencies or departments did you reach out to and did they express interest or commitment?
SportSG ActiveSG A&C and ITD are interested in supporting the system post-hackathon.
# Solutioning
## Problem-Solution Fit
How does your product specifically address the pain points identified?
SportsAssist digitizes attendance and assessment, replacing paper with a unified online system. An AI agent auto‑drafts personalized comments and remarks from feedback for the current season, enabling coaches to quickly review and share with parents. All student assessment data is centralized, giving ActiveSG A&C powerful analytics to uncover programme insights and drive continuous improvement. The result: faster reporting, smarter feedback, and data‑driven growth across the entire academy network.
## Functionality
What are your key user flows/features?
SportsAssist – Core User Flows
1. Attendance Taking
  - Head, Lead, or Assistant coaches login to capture session attendance.
  - Option to upload MC for traceability and eligibility computation.
1. Student grouping for assessment
  - Head coaches login to organizes participants into teams based on participants' skill levels.
1. Skill assessment for Students
  - Assistant coaches login to select team to record actual timing or counts.
  - Scores are instantly computed using pre‑configured rubrics for consistency.
1. Review of Progress Reports
  - Head coaches login to review the detailed assessment by season.
  - Head coaches can review and edit the initial AI‑drafted comments to be shared with parents.
1. Release of Progress report to Parents
  - Head coaches can schedule or instantly publish progress reports by season.
  - Parents login to view their child’s assessment reports.
  - Centralized data ensures transparency and enables collection of multiple seasons of data for ActiveSG A&C to analyze insights across programmes for future planning.
## User Experience
How did you make the experience seamless/intuitive for the end user?
1.  Coach efficiency
  Coaches get an instant overview of student attendance, with flexible grouping tools that eliminate
paperwork and allow quick adjustments.
1. Assessment flow
  Live scoring is streamlined with pre‑configured rubrics, ensuring consistency and reducing
manual effort.
c) AI‑powered comments and remarks
  An AI assistant drafts tailored comments and remarks based on feedback provided by the coaches for the season, giving coaches a head start in drafting insightful comments and remarks.
d) Parent satisfaction
  Progress reports are easier to access, and delivered on time — boosting trust and
engagement with the programme.
## User Validation
What feedback did users give about the product? What worked well and what required improvement?
1. Usability Test with 4 coaches:
  The prototype was well received, with overall experience ratings averaging 8.5/10, challenge addressal averaging 8.25/10, and intuitiveness averaging 9/10 across the four coaches.

What Worked Well

The standout feature was the automation of report generation, with one coach specifically highlighting AI-generated comments for Head coaches to edit as the most valuable aspect. Another coach praised the automated conversion of scores, noting it eliminated the need for paper-based processes. The system was described as "fast and much easy to use" and "user friendly." Perhaps the most telling endorsement came from a basketball coach who said they been wanting a solution and felt they could "use it immediately" — reflecting how long coaches have felt the pain of the current manual process.

What Required Improvement

The only specific improvement raised was the addition of a spelling check for assessment comments. No other structured improvement feedback was provided by the remaining coaches.

Adoption Intent

All four coaches indicated they would adopt the digital solution, with scores ranging from 7 to 10 out of 10, suggesting strong readiness for rollout.
1. Feedback from SportSG Admin (10 submissions):
  What Worked Well
  The prototype received consistently high scores across all three rating dimensions — overall impression, addressing key challenges, and data insights potential — with no score falling below 8 and most sitting at 9 or 10. Respondents were particularly positive about the automation of progress report generation and dissemination to parents, which directly reduces the manual workload on coaches. The centralisation of attendance, assessments, and reporting into a single platform was widely praised, with staff appreciating that they no longer need to navigate fragmented systems. The clean interface and standardised templates across all sports were also highlighted as strong points.
  What Required Improvement
  Automated trend reporting and actionable insights were the most commonly requested additions. Other gaps included head coaches needing rights to manage their own coach rosters, tracking a child's progression across seasons, audit timestamps, and coach timesheet management.
  Insights
  Staff aren't just looking for a digital replacement of current processes — they want the platform to surface intelligence for better programme decisions and identifying poten. Investing in trend analysis and automated reporting would have the highest impact.
# Impact & Next Steps
## Success Metrics
What is your "North Star" metric?
Every ActiveSG A&C coach digitally captures participant assessment data across all sports every season, so that timely and actionable progress reports reach every parent and administrator, driving better programme decisions and growing the next generation of sporting talent.
- Progress reports delivered The number of reports generated and shared with parents. A consistently high figure demonstrates strong coach adoption and proves the platform is genuinely useful.
- Assessment‑to‑report time The average time from capturing assessments to finalizing reports. A low duration highlights meaningful time savings for coaches, allowing them to spend more energy on training rather than administration.
## Expected Impact
What outcomes do you expect this to be able to deliver in the short/medium/long term if your product is launched to users?
Short term: More than 50% reduction in time spent by coaches from preparing the progress reports to reviewing and sending.
Long term: Driving better programme decisions and growing the next generation of sporting talent by ActiveSG A&C.
