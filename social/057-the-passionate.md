---
title: "The PAssionate - PAssion CARES Xpress"
description: "Be a PAssion member instantly - Earn Points and Do Good for the community!"
sidebarTitle: "The PAssionate"
icon: "users"
---

# The PAssionate - PAssion CARES Xpress

| Field | Value |
| --- | --- |
| Requested team | The PAssionate |
| Judging group | Final Judging Group 3 |
| Scheduled time | 2:56pm |
| Team number | 57 |
| Category | Social |
| Booth | 8E-15 |
| Project page | [https://build.tech.gov.sg/projects/2026/57](https://build.tech.gov.sg/projects/2026/57) |
| Product link | [https://go.gov.sg/passion2026](https://go.gov.sg/passion2026) |
| Team members | Chinn Woan Tan; Elizabeth Chia; Elizabeth Orbe Lumban; Jennifer Lin; Kwok Leong Lam |

## Summary

Be a PAssion member instantly - Earn Points and Do Good for the community!

## Full Write-Up

# Problem Statement
## Users
Non-PAssion members who attend PAssion CARES events, representing a pool of up to ~2 million Singapore residents with untapped membership conversion and community giving potential. Those who show up at events are residents who have already chosen to participate in their community. Yet the current flow fails to capture them at the moment of highest interest.
PA hosts ~55,000 events annually with over 1.8 million attendees in 2025 alone, of which PAssion CARES events made up ~20,000 events with ~1 million attendees.
## Use Case
When a non-PAssion member arrives at a PAssion CARES event, they want to participate, do good, and earn rewards — just like any existing member. They encounter this problem at the moment of highest interest: at the event itself, when they scan the PAssion CARES event QR code and are immediately redirected into a membership sign-up flow instead of being able to participate seamlessly.
PAssion CARES loyalty programme — launched in July 2018 and supported by sponsors i.e., yuu Rewards Club/POSB — rewards each successful scan with 10 Yuu Points credited to the participant's account and 10 Yuu Points contributed to community projects, matched by sponsors. Non-members are currently locked out of both until they complete the full membership registration process. PAssion e-membership was introduced in June 2025 as the fastest path to membership, but the current PAssion CARES event QR flow has yet to deliver on membership conversion.
## Pain Point
Each willing participant who is a non-PAssion member, despite being present and interested in doing good while earning reward points, faces a fragmented registration journey of up to 15 minutes to be a PAssion member before they can participate and access rewards. This friction at the moment of highest intent causes participants to lose interest or abandon the process entirely.
The PAssion CARES event participation system was designed exclusively for existing Principal members, creating a closed-loop experience that does not accommodate seamless membership conversion.
Even with the introduction of e-membership in June 2025 — designed to be the fastest path to membership — the PAssion event QR flow still redirects non-members into a lengthy process, failing to deliver on membership conversion at the most critical touchpoint.
The reward system is exclusively tied to existing member credentials (PAssion membership CAN ID for Yuu points), forcing interested non-members participants to endure lengthy administrative processes to be a member or forgo the community giving opportunity and personal rewards entirely.
## Consequence
The cost of inaction is broken membership conversion at the worst possible moment — when residents are already present, motivated, and ready to participate.

Of the ~2M non-PAssion members in Singapore, those who show up at PAssion CARES events are the warmest leads for membership conversion — yet only 12% (~3k of 25k) e-membership sign-ups in the last 10 months came from PAssion CARES event QR redirects. The remaining 88% signed up through other channels, on their own time, without the pressure of signing up at the event even though events should be driving far more conversions than this.

This is not just a lost membership opportunity. Sponsors matching successful scans contributed ~$100,000 to community projects last year alone; every failed conversion at an event directly reduces what communities receive — leaving the ~2M largely untapped and community impact below its potential.
# User Research and Market Analysis
## User Research
What user research methods did you adopt to validate that this solution is needed and what were the key insights from real users?
Non PAssion members struggle to sign up for membership to earn and contribute to the community at PAssion CARES events.
Initial research insights:
- Guerilla user research – 15 users at events.
- Current process relies on pulling these users to one side at the event and guide them through the sign-up process before scanning the event QR code again to earn rewards and do good.
- There is high demand for a straightforward process to sign up quickly at the event and get the points.
- Considerations include users with mobile devices with low battery and the urgency to get into the events with their families and friends.
Three user personas were identified through interviews and observation studies, each representing a distinct friction pattern:
- David (25, Young Professional): Completed sign-up but found the journey fragmented across 3 apps. Motivated by sunk cost — stayed because he felt he had to justify the effort. Pain: unclear value proposition before sign-up.
- Mary (50, Working Professional/Mother): Almost left three times during registration. Relied on her daughter's help to complete the process. Pain: multi-step complexity and immense time pressure at event entrances.
- Sarah (16, Student): Carries a portable charger to events because a dead phone means no participation. Pain: absolute lack of offline backup systems and poor mobile connectivity at venues.
Three core themes emerged across all profiles: time pressure, technological complexity, and the influence of peers and family. The primary reason residents were able to complete the membership sign-up was not due to good UX but human intervention. Key pain points centered on fragmented flow and the stress of registering while the event is about to start or had already started.
Ground observation at a recent event (with total ~232 attendees) found about 40% of scans unsuccessful, corroborating the interview findings at scale.
## De-risking
What market risks are there and how did you mitigate them?
Two core hypotheses were tested:
1. Residents are not signing up because of the lengthy membership sign-up process. ~40% unsuccessful scans at recent event and only ~300 monthly e-membership conversions attributed to event QR codes over the past 10 months.
- Mitigation: Implement minimal and deferred onboarding. The flow asks for consent to retrieve minimal requirements via MyInfo, users can instantly submit and be a member while doing good and getting rewarded.
1. Residents are not signing up due to the lack of information on what they are missing out on. Knowing that each scan earns personal Yuu Points and contributes to community projects gives non-members a concrete, immediate reason to sign up on the spot.
- Mitigation: Put up information upfront to nudge people to sign up and do good!
## Stakeholder Buy-in
Which agencies or departments did you reach out to, and did they express interest or commitment?
PA Membership & Partnership (M&P) is the problem owner and active participant (Augustine Tan) in this hackathon, with ongoing engagement validating operational pain points and confirming interest in streamlined solution. Yuu Rewards Club and POSB are existing partners in the PAssion CARES ecosystem.
# Solutioning
## Problem-Solution Fit
How does your product specifically address the pain points identified?
PAssion CARES Xpress eliminates the multi-step membership registration journey by handling the backend membership and points crediting after a single SingPass authentication. Non-members can immediately be converted into members and participate in the community giving mission — contributing 10 Yuu Points to community projects and earning 10 Yuu Points for themselves — without leaving the event flow.
## Functionality
What are your key user flows/features?
The streamlined guest participation flow delivers a seamless event experience in 5 steps:
1. Non-member scans PAssion CARES event QR code.
1. User logs in with SingPass.
1. System retrieves MyInfo data automatically — no manual form filling.
1. User is shown pre-populated details, consents to signing up for PAssion membership and submits to do good and get rewarded with Yuu points.
1. Success screen confirms "Event reward added to your account — you've also contributed to your community!" with option to complete profile later for more perks and cashing out their Yuu points.
All backend processes — membership sync and community giving points — happen automatically in the background. The user does not need to wait or re-scan the event QR.
## User Experience
How did you make the experience seamless/intuitive for the end user?
The flow reduces the journey from 15 minutes to under 2 minutes with 1 scan. Profile completion is deferred to post-event and incentivised with bonus points, removing the pressure of completing administrative tasks during the event. The dual reward message (personal Yuu Points + community contribution) is surfaced upfront to address the unclear value proposition identified in user research.
## User Validation
What feedback did users give about the product? What worked well and what required improvement?
Prototype usability testing conducted with PA staff and mock event scenarios. Feedback incorporated into the 5-step flow and the following clarification from Business user affirmed the prototype:
- Once a member scans the PAssion event QR code, points are credited immediately.
- If they haven't linked their Passion membership to a Yuu account, points are held in a shadow account and automatically transferred once linked.
- Even without linking, the sponsor match still counts as a valid participation, meaning the community donation still goes through.
# Impact & Next Steps
## Success Metrics
What is your "North Star" metric?
e-membership conversion rate at events — the percentage of non-member PAssion event attendees who successfully complete e-membership sign-up during the event.
- A rising conversion rate indicates that the friction barrier has been meaningfully reduced, and that residents who show up at events — already the warmest leads — are successfully captured at the moment of highest interest.
We will also track the following supporting metric:
- Time to complete sign-up (target: under 2 minutes) — a direct measure of whether the experience is genuinely faster and simpler than before.
- Sponsor-matched Yuu Points contributed to community projects (baseline: ~$100,000/year) — a measure of whether more community giving is happening as a result.
## Expected Impact
What outcomes do you expect this to be able to deliver in the short/medium/long term if your product is launched to users?
Short term: Pilot across 3-5 PA events for ~3-6months targeting a 3x increase in monthly event-attributed memberships (from ~300 to ~1,000/month). Every new member also unlocks a new community contributor — meaning more Yuu Points funds matching from sponsors flowing to community projects per event.
Long term: If sustained across ~22,000 annual events, PAssion Cares Xpress has the potential to meaningfully convert a portion of the 2 million untapped residents into active PAssion CARES participants, amplifying both personal engagement and community impact.
