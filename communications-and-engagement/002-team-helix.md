---
title: "Team Helix - Helix Bot"
description: "~7k SWDA cases/month aren’t triaged early; 10.29% run over 60 mins, results in missed opportunities for SWDA to deliver good citizen service."
sidebarTitle: "Team Helix"
icon: "users"
---

# Team Helix - Helix Bot

| Field | Value |
| --- | --- |
| Requested team | Team Helix |
| Judging group | Final Judging Group 1 |
| Scheduled time | 2:03pm |
| Team number | 2 |
| Category | Communications and Engagement |
| Booth | 1E-16 |
| Project page | [https://build.tech.gov.sg/projects/2026/2](https://build.tech.gov.sg/projects/2026/2) |
| Team members | Alvina Lee; Keat Jau Yaw; Kee Weil Lim; Wei Liu; Wen Kai Ang |

## Summary

~7k SWDA cases/month aren’t triaged early; 10.29% run over 60 mins, results in missed opportunities for SWDA to deliver good citizen service.

## Full Write-Up

# Problem Statement
## Users
~4.8k individual citizens per month, ~ 20 Customer Service Agents
## Use Case
Citizens contact SWDA needing to get to the right help channel quickly, especially for ambiguous and routing-heavy enquiries. Officers need a way to distinguish routine enquiries that can be redirected or self-served from heavier cases that require human handling. The triage opportunity is most visible in five high-volume categories where enquiries are less structured and more likely to require better routing at first contact:
• SkillsFuture Credit — 34,946 cases, 25.32% abandonment
• Appointment (Booking / Reschedule / Cancel) — 5,068 cases, 6.27% abandonment
• Appointment (New) — 2,220 cases, 8.02% abandonment
• Employment Facilitation — 1,261 cases, 42.82% abandonment
• Career Guidance — 501 cases, 11.18% abandonment
## Pain Point
Citizens do not know whether they will get quick help or end up in a longer, more fragmented journey when they contact SWDA.
Many enquiries are simple and could be resolved quickly, but they are not separated early enough from heavier cases at intake. As a result, citizens land in the wrong queue, wait longer than necessary, or need follow-up through callbacks, missed calls, or voicemails before reaching the right support.
Our survey of 96 hotline users confirms this: “getting to the right help quickly” was the single most important factor (54 / 96 respondents), and the top two frustrations were long waiting time / queue uncertainty (41) and not knowing which menu option to select (31).
## Consequence
Without early triage, simple enquiries continue to enter human-assisted queues unnecessarily while complex enquiries are not routed fast enough to the right support path. This increases queue pressure across ~89,293 call cases annually and shifts operational effort toward follow-up and recovery instead of first-contact resolution.
The burden is not only volumetric but also inefficient. Callback-related cases have a 10x longer median handling time and are 3.44x more likely to exceed 60 minutes than routine cases — so failed or poorly routed journeys consume significantly more officer effort than the cases they replace. Left unsolved, the recovery tail keeps growing while officer capacity stays flat.
# User Research and Market Analysis
## User Research
We combined quantitative and qualitative methods to validate the problem and de-risk the solution direction:
•        Quantitative survey (n = 96): “Your Experience
Calling Service Hotlines” — covered hotline usage, frustrations, willingness to use AI triage, and preferred fallback. Skewed toward 35–54 (62 of 96 respondents), with 59 having called a hotline in the past 6 months.
•        Operational data analysis: 89,293 SWDA call cases analysed across 5 high-impact enquiry categories to identify abandonment hotspots and recovery cost.
•        Moderated prototype testing (Helix bot): structured 6-step session with at least 10 users, 35 (SkillsFuture Credit appeal status). Tested intake menu, AI recommendation, Singpass authentication, and routing journey to see if the user as a citizen will be able to accept such journey
Key insights:
•        Strong appetite for the solution: 62.5% of respondents said they would use an AI voice triage option, and a further 31.2% said “Maybe” — only 6.2% said “No”. Average usefulness rating: 4.03 / 5.
•        What users value most: Faster routing to the right team (71 / 96), shorter wait time (60), and ability to solve simple queries immediately (43).
•        Trust is the constraint, not appetite: Trust in AI to handle enquiries accurately was 3.12 / 5. The top concerns were “AI may misunderstand me” (63), “I prefer a human agent” (47), and “unsure if AI answer
is reliable” (46).
•        Universal fallback expectation: Across nearly every respondent, the preferred fallback when AI cannot help is “transfer me to a human agent with context” — this is non-negotiable.
## De-risking
Helix rests on three assumptions, each with a corresponding mitigation:
•        Demand risk — will citizens use AI triage instead of waiting for an agent?
Validated: 93.7% of survey respondents said Yes or Maybe, and “faster routing” ranked as the #1 desired benefit. Survey skews toward 35–54 (the dominant SWDA caller cohort), so demand signal is representative.
•        Trust risk — will users trust AI on a sensitive query (e.g. SFC appeal)?
Trust score is moderate (3.12 / 5) and the dominant concern is misunderstanding. Mitigations built into the flow: (i) a confirmation read-back loop after voice capture so users can correct misclassification before routing; (ii) Singpass authentication for any case-specific information, anchoring the interaction in an identity
verification users already trust; (iii) AI disclosure at session close per moderator script; (iv) a one-tap fallback to a human agent with full context attached — the universally preferred fallback in our data.
•        Adoption risk — will officers and SWDA leadership adopt the workflow?
Helix is designed to remove the most painful queue (callback / recovery cases, which are 10x more expensive in handling time) rather than displace officer judgement. Officers retain full handover context in the CRM — “the agent answers with no context” state is exactly what Helix eliminates.
## Stakeholder Buy-in
SWDA is the primary business owner and has provided the case-volume dataset, abandonment baselines. 
This will be POC as one of the AI components in the agency's Voice+ Project, which is a cloud telephony system.
# Solutioning
## Problem-Solution Fit
Each layer of Helix maps directly to a validated pain point:
•        Voice intent capture → removes the “didn’t know which option to select” frustration (31 / 59 callers). The user describes their enquiry in their own words instead of navigating multi-level IVR menus.
•        AI classification with read-back confirmation → addresses the #1 user concern (“AI may misunderstand me”, 63 respondents). The system says back what it heard, and the user confirms or corrects before routing.
•        Singpass authentication → unlocks personalised, case-specific resolution (e.g. SFC appeal status) without re-explaining identity to a human agent.
•        End-to-end resolution with email confirmation → closes routine cases at first contact, removes them from the human queue, and addresses the recovery tail (~2,635 callbacks/year, 10x longer handling time).
•        Warm handover to a human officer with full CRM context → satisfies the universally preferred fallback (“transfer me to a human agent with context”), so users never have to re-explain.
## Functionality
Generic flow (applies across all journeys):
•        Caller dials the SWDA hotline. AI greeting + language selection.
•        AI prompts: “Please briefly describe your enquiry.” Caller speaks naturally; AI transcribes and reads back the classified intent for confirmation.
•        Caller authenticates: Singpass for individuals (push notification or NRIC/FIN), Corppass / UEN for employers. Training Providers route directly to TPGateway without authentication overhead.
•        AI either resolves end-to-end (returns the answer + sends confirmation email + auto-closes the case in CRM) or warm-transfers to an officer with the full intent, transcript, and auth context attached.
Six specific journeys built into the prototype:
•        Individuals — Check SkillsFuture Credit balance: Singpass auth, balance returned in-call, email confirmation. Self-served, no officer.
•        Individuals — SFC unlisted-course appeal: identified as a complex case during triage; routed to manual review with full intent and attachments captured up-front so the citizen never has to repeat themselves.
•        Individuals — Career advisory / upskilling pathway: guided conversation; personalised recommendations dispatched by email post-call.
•        Employers — SDL computation / appeal: UEN verified via Corppass; SDL details retrieved or escalated cleanly to the right team.
•        Employers — SFEC enquiry: enterprise-credit information returned with case automatically created for any follow-up.
•        Training Providers — e-Attendance appeal: direct routing to TPGateway, no SWDA officer transfer required — a class of cases that today consumes officer time as pure handoff.
A live interactive prototype of all six journeys is available at the URL above.
## User Experience
•         Speak, don’t navigate: the caller describes the enquiry in their own words instead of guessing at IVR categories.
•        Confirmation, not assumption: the AI reads back what it understood before any routing decision — a deliberate response to “AI may misunderstand me” as the top user concern.
•        Singpass / Corppass instead of identity questions: callers authenticate through apps they already trust, with one tap, instead of answering NRIC / UEN / DOB sequences over the phone.
•        Resolution by email: for routine enquiries the caller leaves the call with a written confirmation — the “official response”that respondents repeatedly asked for in open feedback.
•        Always a human exit: a human-agent fallback with full context is one tap away at every step. This is the single most important trust feature according to our survey.
•        Direct routing where it makes sense: SFC credit submission routed straight to the SFC portal for direct follow up
## User Validation
Two moderated user testing sessions on 8 May 2026: Session 1 with an individual citizen caller navigating the SFC appeal status flow; Session 2 with a GovTech evaluator reviewing all six journeys across Individual, Employer, and Training Provider segments.
Worked well:
•        Voice intent capture was immediately intuitive.
Both participants understood what to do when prompted to describe their enquiry in natural speech — neither asked what the system wanted from them at this step.
•        Customer type selection was clear.
The initial menu distinguishing Individuals, Employers, and Training Providers was understood without confusion.
•        Singpass authentication was trusted without hesitation.
Both participants accepted Singpass as the identity verification method. Neither raised concern about the notification itself — it was treated as standard practice for government services.
•        Confirmation read-back was accepted.
Participants did not push back on the AI reading back their classified intent before proceeding; the confirm-before-routing pattern was treated as reasonable.
•        Material improvement over the status quo.
Participant 1 (citizen caller) confirmed the prototype would help them get assistance faster than current hotlines, particularly with self-service. Participant 2 (GovTech evaluator) validated the core triage logic and the direction of value: reducing manual effort, shortening queue pressure, surfacing officer context at
handover.
•        Urgency validated independently.
Participant 2 unprompted surfaced the duplicate-case problem (“an impatient citizen calls every day, the CSO sees four separate cases with no linkage”), confirming from an operational lens the pain point Helix is designed to solve.
Required improvement (and how we are addressing it):
•        Enquiry type taxonomy needs more depth.
Callers whose enquiry doesn’t fit a listed category may misroute themselves.
Fix: expand the option taxonomy and add a visible “none of these” / free-text fallback path.
•        Bot identity must be explicit.
“Helix” did not appear in the prototype interface.
Fix: introduce the bot by name at the opening greeting (“Hi, I am Helix”), use first-person language throughout, and avoid generic “AI assistant” framing. A named persona also enables a wake-word
pattern for noisy environments.
•        Pre-verification before Singpass push.
Sending a Singpass push without confirming the caller’s identity creates a false-positive notification attack vector.
Fix: add a lightweight pre-verification (e.g. date of birth or partial NRIC) before triggering the push.
•        Caller persona lock-in.
The prototype allowed users to switch between Individual and Employer mid-session, mismatching the
authentication method (Singpass vs Corppass).
Fix: once a caller type is selected and authenticated, lock the session to that persona; switching
requires a session restart.
•        Remove voice-based email collection.
Spelling out an email by voice is unreliable, unverifiable, and an abuse vector for sending notifications to third parties.
Fix: for authenticated users, use the registered email on file.
•        Appointment rescheduling routes to a CSO.
Real-time availability matching against flexible citizen preferences is not something the bot can negotiate cleanly.
Fix: bot handles appointment cancellation; rescheduling is escalated to a CSO with pre-populated context.
•        Callback should be queue-conditional, not default.
A two-working-day callback for a sub-one-minute enquiry is a worse experience than holding.
Fix: surface callback only when queue length or wait duration exceeds a threshold (subject to Amazon Connect queue-querying feasibility).
•        Duplicate case deduplication.
Repeat callers today generate unlinked cases.
Fix: link cases by caller identity + intent + recency window so repeat contacts append to an existing case rather than spawning new ones — this maps directly to the repeat-contact rate metric below.
•        Training Provider flow should be triage-only.
All TP cases route to a CSO regardless, so bot “resolution” adds complexity without deflection value.
Fix: limit the TP flow to structured context capture (intent, course ID) so the CSO receives a pre-populated case summary.
•        WhatsApp handoff requires explicit caller confirmation.
Not every mobile number has WhatsApp (corporate lines, dual-SIM users).
Fix: before initiating a WhatsApp handoff, prompt the caller to confirm — if not, offer queue or callback.
# Impact & Next Steps
## Success Metrics
Of all inbound calls, the proportion that reach either a resolution (self-served or officer-handled) or a structured fallback (voicemail, callback, transfer) — versus disconnecting with nothing.

We track the supporting metrics below across two cuts: by stage in the value chain (input → output → outcome), and by how quickly they respond (leading vs lagging).
Input metrics (activity we control):
•        % of inbound calls routed through Helix: share of total SWDA hotline volume that enters the orchestrator vs. the legacy IVR. Tells us whether the deployment surface is large enough to draw conclusions
from.
•        Number of intent-confirmation attempts per call: how often we ask the caller to confirm or correct the classified intent. A direct measure of operational load on the read-back loop.
•        Authentication attempt rate: Singpass / Corppass push notifications triggered per call routed. Surfaces wasted attempts after pre-verification is added.
Output metrics (immediate results of those inputs):
•        AI intent classification accuracy: % of voice-captured intents confirmed correct by the caller (press-1) or the officer on CRM review. Direct measure of triage quality.
•        Context pre-population rate: % of officer-handled callback and voicemail cases arriving with intent, IVR path, and transcript already in CRM before officer first-edit. Target 100%.
Outcome metrics (the change in user / officer experience):
•        Self-served resolution rate: % of inbound cases resolved at first contact without an officer. The single most important outcome metric for SWDA.
•        Median Average Handle Time (AHT): for officer-handled cases, especially callback / recovery cases (current: 10x routine). Falls as context pre-population rises.
•        Hotline abandonment rate: on the five high-impact categories (current weighted ~25%, dominated by SkillsFuture Credit at 25.32%).
•        Repeat contact rate: % of cases reopened or duplicated within a recency window. Validates the deduplication fix from Session 2.
•        Citizen post-call satisfaction: survey-style rating after Helix-handled and Helix-routed calls.
Leading indicators (move first, predict the rest):
•        AI intent classification accuracy — visible from week 1; misclassifications cascade into bad routing, low Singpass approval, and abandonment downstream.
•        Context pre-population rate — visible immediately from CRM; predicts officer AHT improvement that follows weeks later.
•        Citizen post-call satisfaction — in-the-moment signal that precedes lagging volume metrics.
Lagging indicators (move later, confirm the impact):
•        North Star — % reduction in unresolved disconnects: only meaningful after several weeks of steady volume.
•        Hotline abandonment rate: requires a baseline period and seasonal correction; expect a 4–6 week confirmation window.
•        Median AHT (officer-handled): changes after officers adapt to the new context-rich handover — typically 6–8 weeks.
•        Repeat contact rate: requires a defined recency window (e.g. 14 days), so trend signal lags by at least that window.
## Expected Impact
Short term (0–3 months — pilot):
•        Pilot Helix on the SkillsFuture Credit category — highest volume (34,946 cases) and highest abandonment (25.32%) — with a clear, measurable target: reduce abandonment by 5 percentage points and resolve >30% of inbound SFC enquiries without officer intervention.
Medium term (3–9 months):
•        Extend Helix to Appointment (Booking / Reschedule /Cancel), Appointment (New), Employment Facilitation, and Career Guidance — the remaining four high-impact categories.
•        Reduce overall recovery-signalled cases by 30%, freeing officer capacity for genuinely complex matters.
•        Bring median AHT for callback / recovery cases closer to the routine baseline by eliminating context loss at handover.
Long term (9–18 months):
•        Helix becomes the default front door for SWDA hotline contact, with seamless escalation to officers for complex cases only.
•        Pattern is portable: the same triage + Singpass + warm-handover stack can be offered to other high-volume government hotlines, multiplying the impact beyond SWDA.
