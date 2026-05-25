---
title: "Data Planters - SurvAI"
description: "An AI-assisted survey workflow platform that helps public officers design the right surveys, test them before launch, and turn responses into insights"
sidebarTitle: "Data Planters"
icon: "users"
---

# Data Planters - SurvAI

| Field | Value |
| --- | --- |
| Requested team | Data Planters |
| Judging group | Final Judging Group 2 |
| Scheduled time | 1:10pm |
| Team number | 111 |
| Category | Productivity |
| Booth | 8F-11 |
| Project page | [https://build.tech.gov.sg/projects/2026/111](https://build.tech.gov.sg/projects/2026/111) |
| Product link | [https://survey.assist.mlops.im/](https://survey.assist.mlops.im/) |
| Team members | Becca Qiu; Biao Yi Pang; Fabien Blanchais; Jun Wei Koh; Wykeith Ng |

## Summary

An AI-assisted survey workflow platform that helps public officers design the right surveys, test them before launch, and turn responses into insights

## Full Write-Up

# Problem Statement
## Users
Public officers across WOG who design, conduct, or analyse surveys. Surveys are widely used across agencies, but most teams lack standardised workflows or dedicated survey expertise.
## Use Case
Officers use surveys to collect meaningful data for decision-making. However, the end-to-end process from survey creation to actionable insights remains manual and fragmented , from question design to analysis and reporting.
## Pain Point
- Survey design is time-intensive with limited guidance, leading to weaker designed questions and lowerdata quality
- Design issues are discovered too late, only after responses are already collected
- Data analysis is manual and slow; officers must set up scripts and functions for every new survey
- Insights are inconsistently derived and dependent on the individual analyst
- Officers have no visibility into surveys already conducted by other agencies, leading to duplicated effort
- There is no easy mechanism to share survey questionnaires or results across agencies or departments
## Consequence
Manhours are wasted across the full survey lifecycle. Ineffective survey design can lead to unreliable insights that undermine decision-making. Duplicate surveys across WOG also reduce opportunities to share report insights for learning and reuse.
# User Research and Market Analysis
## User Research
We validated the problem through a quantitative user survey and qualitative stakeholder interviews.
User survey findings confirmed widespread pain across the survey lifecycle:
- 30–35% of respondents take over a month to design a survey, while 40–45% spend 1–2 months on analysis alone.
- Top challenges includes difficulty extracting clear insights (~25%),manual analysis (~25%), and inability to reuse or compare past surveys (~20%)
- These translate into downstream impact: 35% report delays in decision-making, 30% have lower confidence in their insights, and 22% face increased manual workload.
- FormSG is the dominant tool (~63%), meaning our target users already operate within the government forms ecosystem.
[image](https://wjbbfxaztzhszi7i.public.blob.vercel-storage.com/collab-media/cmnwsadmb001y04jukvy1wh02/019e11c9-8a2e-771c-8d60-1963969edea6-image.png)

Qualitative interviews added depth to these numbers:
- Interview with Dev survey team: Confirmed the multi-step analysis burden. In today's process, the survey lead does high-level analysis, PMs do product-specific analysis, then a writer synthesises the final report. Even the survey expert still manually dumps qualitative comments into AI tools such as AWS Quicksight for summarisation. The pain is real even for power users; it is worse for smaller teams and PMs without dedicated survey expertise.
- Interview with FormSG Product manager, UX designer and engineers: FormSG previously built an AI chatbot MVP for survey insights but deprioritised it. Users knew what outcomes they wanted but were stuck on what to ask, pointing to a need for a more guided, structured interface. They are open to collaboration.
## De-risking
The top market risks centre on AI reliability and scope overlap. To reduce hallucination and inconsistent outputs, statistical guardrails (i.e. sample size and significance thresholds) were built in, while deterministic scripts for quantitative analysis and the LLM is limited for qualitative summarisation only.
We also approached synthetic user simulation carefully. Rather than treating AI-generated responses as a proxy for real data, the goal is to surface whether questions will yield reportable, and comprehensive coverage before the survey goes live.
On the competitive side, we differentiate from existing hackathon projects (Charts, Insight, Delightful Dashboards) by targeting the end-to-end workflow rather than one-off visualisation, and the survey data showing 45% of users run surveys rarely strengthens our case — infrequent practitioners are likely to benefit more from AI assistance.
## Stakeholder Buy-in
- Confirmed Business owner: The team met up with Senior Director of Data Programme, Kevin Ng, who has agreed to sponsor the project in the current stage as business owner.
- Dev survey team: Validated the analysis bottleneck from first-hand experience. Interested to visit the Feedback Bazaar booth to evaluate the prototype.
- FormSG product manager, designer, engineers: Independently arrived at the same problem space and built a prior MVP. Expressed openness to building together, and provided concrete product direction feedback including refining our target user definition and differentiating from the hackathon projects.
# Solutioning
## Problem-Solution Fit
Each pain point from the problem statement maps directly to a built feature
- Survey design is slow with limited guidance → AI Grill Chat refines the survey purpose and target audience through a structured multi-turn conversation before any question is written, ensuring officers start with clarity rather than a blank canvas.
- Design flaws discovered too late → A series of AI-assisted chat modals throughout the design flow (purpose refinement, structure refinement, audience chat) surface issues at each stage rather than after fielding. Gap analysis is one of these, flagging missing topics, weak questions, and validation gaps on demand. Persona Simulation adds a further pre-launch check, running the survey against a synthetic respondent population to catch structural issues before real responses are collected.
- Manual, inconsistent analysis → Response Import with automated Report Generation eliminates per-survey scripting. Deterministic scripts handle quantitative distributions; the LLM is reserved for qualitative summarisation, keeping outputs consistent across officers and teams.
[image](https://wjbbfxaztzhszi7i.public.blob.vercel-storage.com/collab-media/cmnwsadmb001y04jukvy1wh02/019e11ca-cd7e-72de-b593-0eeffa0034df-image.png)
## Functionality
The core user journey unfolds across four stages
1. Define — The Grill Chat walks the officer through purpose, audience, hypotheses, and constraints. Output: a refined title, purpose statement, and audience description that seeds the AI.
1. Design — AI suggests a full survey structure (sections and question types) from the purpose. The AI Assistant helps to refine each section on demand, flagging missing coverage, question improvements, and validation issues with one-click insertion.
1. Test — Persona Simulation selects demographically relevant respondents from the SG persona library and runs them through the survey, generating synthetic response distributions. Officers can inspect per-persona answers and identify questions that fail to discriminate or confuse respondents.
1. Analyse — After live responses are collected, officers import them via bulk upload. AI-powered report templates auto-generate structured reports (summary, key insights, distributions, data quality) in markdown, ready for use.
[image](https://wjbbfxaztzhszi7i.public.blob.vercel-storage.com/collab-media/cmnwsadmb001y04jukvy1wh02/019e11cb-1104-75ab-96bd-5ed70115df23-image.png)
## User Experience
The interface choices were hypotheses formed during our own research and later confirmed by user interviews
- Grill Chat before design: FormSG team found that users knew what outcome they wanted but were stuck on what to ask. We surfaced this as a structured conversation upfront rather than a blank form, so the AI has a well-specified brief before generating anything.
- Streaming responses: All AI outputs stream in real time via Server-Sent Events, so the interface feels responsive even on longer generations — removing the dead-wait friction of a loading spinner.
- Linear 4-step wizard: The wizard enforces a design sequence (purpose → structure → questions → finalise), preventing officers from jumping to question writing before the survey's scope is clear.
- Guided hints: Contextual AI hints appear within each section during design, reducing the cognitive load of knowing what to ask next.
[image](https://wjbbfxaztzhszi7i.public.blob.vercel-storage.com/collab-media/cmnwsadmb001y04jukvy1wh02/019e11cb-7a18-7729-aa2b-bd9cb46f2e39-image.png)
## User Validation
At the feedback bazaar, we received product ratings from 39 users and 2 pieces of qualitative feedback. Overall, the user ratings indicate that users in general found that our product addresses a clear pain point, is well-executed, and worthy of further investment, with an overall quality score of 4.56/5.
The qualitative feedback is request for additional functionality: users want to be able to further edit the specific report sections, with AI assistance, and to be able to export the survey report in an editable format for further changes.
The solution approach also has directional validation from key stakeholders in the survey space:
- Dev survey team validated the overall direction — even a dedicated survey expert with specialised tooling still hits manual bottlenecks throughout the analysis cycle, confirming the pain is real for power users and worse for smaller teams and PMs without dedicated survey expertise.
- FormSG team independently scoped and built a prior AI MVP for survey insights, arriving at the same problem space unprompted. Their candid deprioritisation of that MVP — due to users being stuck on what to ask, not what outcome they wanted — directly validated the Grill Chat as the right entry point.
# Impact & Next Steps
## Success Metrics
North Star: Time-to-insight — the end-to-end elapsed time from survey creation to a reportable set of findings.
- Current baseline from user research: 35% of officers spend over a month on design alone; 45% spend over one month on analysis. End-to-end, the full survey lifecycle can stretch to 3 months or more.
- Target with SurvAI: 1–2 weeks end-to-end, with the majority of time reduction coming from eliminating manual analysis scripting and catching design issues before fielding (avoiding costly redesign cycles).
## Expected Impact
Short term (0–6 months, based on features already built)
- Officers complete the design-to-insight cycle in 1–2 weeks rather than 2–3 months, recovering significant manhours across the survey lifecycle.
- AI gap analysis and persona simulation shift quality control from post-collection to pre-launch, reducing the rate of surveys that require redesign or yield unreliable data.
- AI-guided report generation accelerates the path from raw responses to presentable findings, removing the need for officers to manually script charts and summaries for every new survey.

Medium term (6–18 months, subject to FormSG integration and broader rollout)
- FormSG integration makes automated response processing the default — officers no longer need to set up Plumber workflows manually for every new survey.
- As the survey library grows within teams and agencies, officers can benchmark new surveys against prior results, reducing redundant design effort over time.
