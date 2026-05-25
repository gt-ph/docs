---
title: "The Missing Layer - Compass for HRBP"
description: "Engineers have GitHub, PMs have Jira, HR has 20 messy spreadsheets and notes. We’re turning HR from person-dependent into resilient and system-driven."
sidebarTitle: "The Missing Layer"
icon: "users"
---

# The Missing Layer - Compass for HRBP

| Field | Value |
| --- | --- |
| Requested team | Missing Layer |
| Judging group | Final Judging Group 1 |
| Scheduled time | 1:10pm |
| Team number | 20 |
| Category | HR |
| Booth | 10C-05 |
| Project page | [https://build.tech.gov.sg/projects/2026/20](https://build.tech.gov.sg/projects/2026/20) |
| Product link | [https://compass-staging.up.railway.app](https://compass-staging.up.railway.app) |
| Team members | Astrina Fitria Rachmat; Hao Wen Tee; Jing Zhi Chan; Max Ng; Shawn Tan |
| Match status | normalized-the |

## Summary

Engineers have GitHub, PMs have Jira, HR has 20 messy spreadsheets and notes. We’re turning HR from person-dependent into resilient and system-driven.

## Full Write-Up

# Problem Statement
## Users
13 HR Business Partners (HRPs) across GovTech supporting multiple clusters and portfolio, scalable to 500+ HRBPs across the Whole.
## Use Case
HRBPs operates as strategic advisors to senior leaders and business units, supporting workforce planning, employee engagement, talent assessments, divisional restructuring and complex employee cases. To perform effectively, HRBPs need access not only to employee records, but also contextual and historical knowledge accumulated through ongoing engagements with divisions and employees.
## Pain Point
Existing HR systems such as Workday, Nexus and Appraise effectively store transactional workforce records, but they are not designed to support the operational workflow of HRBPs. Critical contextual information, such as leadership discussions, employee concerns, organizational sentiments, workforce risks, meeting notes, and follow up actions are fragmented across multiple spreadsheets, presentation decks, email threads, chat platforms, personal notebooks, and individual HRBP memory.
As a result, HRBPs require substantial effort manually consolidating information across disconnected platforms before every strategic discussion or workforce intervention.
## Consequence
These disjointed knowledge leads to inefficient data retrieval and manual cross-referencing across multiple platforms by HRBPs. In worse case, missed information and inconsistent follow-up actions may lead to inaccurate organizational context and wrong advise given to the business. Each HRBP spends ~12.5 hours/week on manual data assembly - over 30% of productive capacity. Across 500+ HRBPs in WOG, that's ~325,000 hours/year. All this time spent reduces time available for higher-value strategic advisory work and proactive workforce engagement.
With no shared operating environment, HR strategic partnership quality also depends entirely on the individual instead of the system. When there is a handover from one HRBP to another, each HRBP takes ~4 months to transition fully and rebuild the portfolio context from scratch, resulting in reduced continuity and degraded service to business leaders.
# User Research and Market Analysis
## User Research
Research was conducted through workflow observations of the day-to-day job scope of HRBPs managing portfolios within SCG. The team consists of 3 team members who are relatively new to the portfolio, and a consistent pattern emerged where:
- HRBPs relied heavily on manual information synthesis
- Contextual knowledge was frequently stored informally
- Collaboration across HRBP team members lacked a shared operational system
One high-frequency workflow identified was the preparation for workforce planning discussions with division leaders:
  Example Workflow Observed
  1. Extract manpower report (in Excel) from Workday and MMF numbers from Tableau dashboard
  1. Massage and clean report manually in Excel to obtain key employee data
  1. Analyze divisional trends such as headcount, manning rate, contract expiry timeline, performance ratings and distributions and further split by departments
  1. Convert findings into visually appealing presentation deck on PowerPoint
  1. Review historical meeting notes and concerns that needs to be incorporated
  1. Check ongoing employee cases handled by different HRBPs that needs to be incorporated
  1. Conduct workforce discussion with division leaders and record notes on note-taking app
  1. Track and coordinate follow-up actions across multiple platforms (i.e. Workday, Nexus, Outlook/Teams/Slack)
  1. Repeat process again before subsequent discussion session
As a highly impactful workflow, this repeated need to manually reconstruct workforce context across systems became a major opportunity area.
## De-risking
Our product hinges on the assumptions that the operational burden of fragmented workforce management is sufficiently painful for HRBPs to adopt a new shared workspace. Focus was placed on mapping actual operational workflows instead of hypothetical ones and augmenting existing systems rather than fully replacing them. As such, the product is intentionally positioned as an orchestration layer on top of existing HR systems, reducing implementation friction and minimizing disruption to current HR processes.
Discussions with CIOO and POS teams also indicated that existing enterprise HR systems are unlikely to evolve significantly in this problem space in the near term, validating the need for a dedicated HRBP operating workspace.
## Stakeholder Buy-in
SCG HRBPs have been heavily involved in the development of the product and will look to adopt it as part of their operational workflow as soon as possible. GDT HRBPs also surfaced interest in piloting the product as a collaborative workspace to centralize portfolio knowledge and team coordination between 4 of them.
# Solutioning
## Problem-Solution Fit
A centralized HRBP platform that brings together live workforce data from HR systems (e.g. Workday, Nexus, Appraise) and HRBP day-to-day process workflow together securely.
Rather than replacing existing systems, the platform acts as a strategic orchestration layer across GovTech’s HR ecosystem while maintaining existing security and access controls. The strategic workspace enables HRBPs supporting a same cluster to
- retrieve workforce intelligence within seconds
- record contextual knowledge systematically
- collaborate and coordinate actions within the team
- conduct workforce planning more effectively
This transforms fragmented administrative workflows into a continuous, context-driven operating model for strategic HR partnership.
## Functionality
1. Dashboard - Consolidated operational view of workforce statistics, upcoming events, attention flags, and prioritized action items for the week.
  - This enables HRBPs to quickly assess business' HR needs and prioritize strategic interventions and their work for the week.
  [image](https://wjbbfxaztzhszi7i.public.blob.vercel-storage.com/collab-media/cmnwnbibx000304jprzlq8kcy/019e590b-1f29-711e-9185-6f81a44e1459-image.png)
  [image](https://wjbbfxaztzhszi7i.public.blob.vercel-storage.com/collab-media/cmnwnbibx000304jprzlq8kcy/019e590b-cf29-70df-8105-43ff7fca5f88-image.png)
1. Meetings - Centralized meeting workspace for HRBPs to capture discussion notes, context, follow-up actions, and workforce considerations in a structured and retrievable manner.
  - Meeting records can be linked directly to divisions, employees and action items via custom tags for recurring themes or categories.
  - In a meeting, HRBP can assign action items in real time for future follow-up without having to keep personal notes on Slack/Teams/email/notebook.
1. Actions - Collaborative action tracking workspace that enables HRBPs to manage operational follow-ups with clear ownership, timelines, and status visibility.
  - Supports coordination across HRBP team members working on the same portfolio, reducing the need for manual follow-ups and disconnected tracking methods.
  - Aggregated action data can also provide visibility into recurring workforce issues, operational workload distribution and areas where HRBPs spend the most time on.
1. Employees - Consolidated view combining Workday, Nexus, Appraise, and Talent Stack data to aid strategic discussions.
  - Related meeting discussions, actions and tags highlight considerations are surfaced alongside the employee records.
  - Enables HRBPs to access structure workforce data and operational data within a single employee list view.
  [image](https://wjbbfxaztzhszi7i.public.blob.vercel-storage.com/collab-media/cmnwnbibx000304jprzlq8kcy/019e590f-bd8f-7749-8c30-db50fd2d5224-image.png)
1. Org Chart - Interactive org chart with team-level visibility beyond existing HR system limitations.
  - HRBPs can navigate organizational structures more intuitively while viewing key employee information, workforce insights, and contextual notes alongside the org structure.
  - Enables HRBPs to identify divisional gaps or risks, quickly surface relevant employees for follow-ups and access contextual information without switching multiple platform.
  [image](https://wjbbfxaztzhszi7i.public.blob.vercel-storage.com/collab-media/cmnwnbibx000304jprzlq8kcy/019e5911-8124-75fa-a3c1-3d1182cdcc42-image.png)
1. Org Chart (Scenario Builder) - Interactive restructuring and planning tool that enables HRBPs to model and facilitate restructuring discussions within the platform.
  - Employee data and workforce considerations are surface in real time, reducing need to manually prepare separate PowerPoint and shuffle between Excel tabs.
  - Shared environment allows for division leaders to visualize proposed restructuring changes, assign tagging, compare scenarios, and assess impact effectively during workforce planning discussions.
  [image](https://wjbbfxaztzhszi7i.public.blob.vercel-storage.com/collab-media/cmnwnbibx000304jprzlq8kcy/019e5912-a2b2-75ad-8465-b19520a6437f-image.png)
Future enhancement:
- AI Transcription feature for Meetings and Actions
- Connection to Slack/Teams notes
## User Experience
The product experience is designed around the HRBPs' day-to-day workflow. Key design principles includes minimizing context switching, simple visuals and enabling seamless navigation across tabs.
Additionally, it links employees, meetings, organizational structures, and action items together within a shared operational environment, allowing HRBPs to move quickly between strategic discussions and operational follow-ups. Colours for visual aids are then introduced to reduce cognitive overhead for HRBPs and ease discussions with divisional leaders.
## User Validation
Initial feedback from HRBPs highlighted strong resonance with the problem space, particularly around fragmented information management, repeated manual preparation work, and lack of continuity. Primarily, users responded positively to a consolidated employee view, the integrated meeting and actions tracking, and the ability to visualize divisional structure alongside workforce context.
One key learning was the importance of linking the data from meeting and actions to the information on the Employees and Org Chart features, which led to iterative refinement of the tagging systems and contextual linking across the platform. Meeting notes structure was iterated to make adding follow-up actions directly a possibility as well.
A great potential benefit highlighted would be when there is a need to handover the portfolio to a new HRBP, the tool will serve as the handover documentation itself. Instead of forwarding multiple email threads or searching them through the DRMS when the previous HRBP has left.
# Impact & Next Steps
## Success Metrics
North Star Metric: 70% reduction in time spent by HRBPs on manual workforce information consolidation and preparation
[table block omitted in flat markdown; see narrativeBlocks in JSON]
## Expected Impact
Expected outcomes upon launching this product centralise around the HRBP productivity and quality of their strategic partnership to the business
### Short Term:
- Centralize fragmented HRBP workflows into a shared workspace
- Reduce repetitive information consolidation effort
- Improve visibility across workforce discussions and follow-up actions
### Medium-Term:
- Improve collaboration and continuity across HRBPs working in the same cluster
- Strengthen organizational memory and portfolio transition processes
- Enable more proactive workforce planning and employee risk management
### Long-Term
- Establish a scalable operating model for strategic HR partnership across GovTech and WOG
- Institutionalize contextual workforce intelligence beyond individual HRBPs
- Enable more data-informed and sustainable workforce strategy discussions within GovTech and across agencies
Check out our pitch deck here (https://docs.google.com/presentation/d/1jUZYIgT6XRFkZoWd2b2ozfcekcEcj6-jqf_A2j6Utbw/edit?usp=sharing) (open to SG-GWS only)
