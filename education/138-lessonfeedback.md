---
title: "LessonFeedback - Dear Teacher"
description: "Dear Teacher lets teachers upload lesson recordings and receive AI-powered feedback in minutes, with optional mentor or peer reviews."
sidebarTitle: "LessonFeedback"
icon: "users"
---

# LessonFeedback - Dear Teacher

| Field | Value |
| --- | --- |
| Requested team | Lesson Feedback |
| Judging group | Final Judging Group 2 |
| Scheduled time | 2:23pm |
| Team number | 138 |
| Category | Education |
| Booth | 9F-02 |
| Project page | [https://build.tech.gov.sg/projects/2026/138](https://build.tech.gov.sg/projects/2026/138) |
| Team members | Kanashima Hatsumi; Nicholas Lim; Ralph Ian Santos; Tasha Yip; Weiling Chen |

## Summary

Dear Teacher lets teachers upload lesson recordings and receive AI-powered feedback in minutes, with optional mentor or peer reviews.

## Full Write-Up

# Problem Statement
## Users
Singapore's 35,000 MOE teachers across 350 schools.
## Use Case
When teachers seek to improve specific aspects of their instructional practice — such as questioning techniques or wait time provided for student responses — they need the ability to review their own teaching, receive informed feedback on key classroom moments, and translate those insights into actionable improvements for subsequent lessons. This need typically arises between formal observation cycles and is often driven by the teacher’s own initiative, ideally within a week of delivering the lesson.
## Pain Point
Teachers receive at most 1 planned formal observation per year as part of annual evaluation. Beyond that, peer feedback is rare for 3 reasons:
1. Logistical friction: Timetable clashes within and across schools make synchronous lesson observation difficult. Teachers can't easily watch each other teach.
1. Summative bias: 98% of principals use classroom observation for appraisal (TALIS 2024). The dominant experience of being watched teach is therefore high-stakes, not developmental.
1. Eroding mentorship: Novice teachers with assigned mentors fell from 54% (2018) to 42% (2024). Deeper collaboration is eroding even as Singapore leads the world in classroom AI adoption (75% of teachers use AI vs OECD avg 36%) and peer trust remains high (94% trust colleagues vs OECD avg 86%).
## Consequence
Without an accessible and low-friction channel for peer and mentor feedback, teachers are often left to improve their practice in isolation, limiting opportunities for timely reflection and continuous growth. Mentor capacity remains a key bottleneck, reducing the scalability of high-quality instructional coaching, while the strong culture of professional trust and collaboration among educators in Singapore remains underutilized. As demand for sustainable, teacher-driven professional development grows, there is an increasing need for a scalable solution that can support continuous improvement across a larger educator base.
# User Research and Market Analysis
## User Research
The team conducted a small pilot involving 7 teachers, each asked to upload at least two lesson recordings. All participants completed the uploads, providing an encouraging early signal of sustained engagement and perceived value in the AI-generated feedback.
In addition, the team ran concept testing sessions with seven teachers to evaluate and rank 15 potential product concepts. Among the concepts tested, Targeted Feedback Requests (average rank: 1.75) and Framework-Based Feedback (average rank: 3) consistently emerged as the highest-rated features.
Key insights from teacher interviews include:
1. Strong perceived value of AI feedback: Teachers consistently rated the AI feedback positively, with scores ranging from 7–8/10 across participants. Several teachers highlighted that the AI surfaced instructional blind spots they had not previously noticed, such as insufficient wait time after posing questions. One teacher also demonstrated measurable improvement in a subsequent lesson after acting on the feedback received.
1. Peer feedback workflow issues were operational, not behavioural: No teachers exchanged peer feedback during the pilot; however, follow-up analysis revealed that this was primarily due to workflow and onboarding gaps, including missing notifications, access restrictions caused by whitelisting, and the absence of collaborator onboarding. Despite this, interview signals indicated strong demand for collaborative workflows such as Professional Learning Team (PLT) discussions, mentor-mentee coaching, and cross-school classroom sharing.
1. Organic adoption signals: In one participating school, the HOD independently began promoting the platform to additional teachers without prompting from the project team, indicating strong perceived relevance.
## De-risking
[table block omitted in flat markdown; see narrativeBlocks in JSON]
## Stakeholder Buy-in
Commitments from Academy of School Teachers Dy and DGE
# Solutioning
## Problem-Solution Fit
Dear Teacher addresses the three pain points directly:
1. Logistical friction → asynchronous video upload + moment-level commenting; no synchronised schedules required
1. Summative bias → peer-led, private-by-default, never repurposed for appraisal
1. Eroding mentorship → AI does the work of surfacing moments worth discussing, scaling beyond 1:1 mentor capacity
## Functionality
[table block omitted in flat markdown; see narrativeBlocks in JSON]
User flow:
1. Teacher records lesson on iPad / phone
1. Uploads directly to Dear Teacher, declares a learning goal
1. AI returns STP-aligned feedback with timestamped moments — typically within an hour
1. Teacher invites a peer to comment on specific moments
1. AI feedback arrive via Telegram with deep links
1. Teacher reflects, applies to the next lesson — within a week, when the same topic is taught again
## User Experience
- Time-to-value: Target: ≤72h to first actionable feedback. Anchor feedback to specific timestamps so teachers can act, not parse.
- Private-by-default: Never repurposed for appraisal.
- AI augments, never grades: Conversational, not dictative. Teachers can ask follow-up questions.
## User Validation
What worked well:
- AI feedback quality (consistently 7–8/10)
- AI surfacing blind spots teachers couldn't see themselves
- STP grounding appreciated across interviews
- Transcript with timestamp navigation
- Measurable improvement loop: teachers mentioned that their 2nd lesson better than 1st
What needed improvement:
- YouTube upload friction → direct upload
- AI off-target feedback → custom prompting
- Framework jargon opaque to junior teachers → tooltips
- Peer-feedback path broken (no notifications) → unblock pack
- AI feels "dictative" → conversational follow-up mode planned
# Impact & Next Steps
## Success Metrics
% of lessons where the teacher reports at least one actionable takeaway.
(An "actionable takeaway" = at least one concrete next-step suggestion, tagged to an STP area.)
## Expected Impact
Short-term (Jan–Dec 2026 — MVP through Pilot):
- Validate that the peer-feedback loop activates when path is unblocked (the central H2 bet)
- Sustain AI feedback quality at ≥7/10 across n≥20 teachers
- Median time-to-actionable-feedback ≤72h
Medium-term (Jan 2027 — Pilot to Cutover):
- Absorb IrisConnect users (~1,000 teachers across 24+ AST schools)
- Absorb LessonLens users in the same window
Long-term (2027+):
- Scale across MOE schools via the cluster structure (SSDs, IPHODs, HOD ICT, PLT leaders as champions)
- Improve the TALIS-measured decline in peer collaboration by giving teachers a low-friction channel for craft-level growth
