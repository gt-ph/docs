---
title: "Operation Tiergehege - PromptGuard"
description: "Helps officers use LLMs safely by detecting privacy leakage, explaining residual risk, and preserving utility through anonymisation."
sidebarTitle: "Operation Tiergehege"
icon: "users"
---

# Operation Tiergehege - PromptGuard

| Field | Value |
| --- | --- |
| Requested team | Operation Tiergehege |
| Judging group | Final Judging Group 4 |
| Scheduled time | 1:53pm |
| Team number | 82 |
| Category | Data & AI |
| Booth | 9B-13 |
| Project page | [https://build.tech.gov.sg/projects/2026/82](https://build.tech.gov.sg/projects/2026/82) |
| Team members | Chong An Chen; James Teo; Judy Hong; Nicole Ren |

## Summary

Helps officers use LLMs safely by detecting privacy leakage, explaining residual risk, and preserving utility through anonymisation.

## Full Write-Up

# Problem Statement
## Users
Our immediate users are public officers and agency teams who send sensitive text into LLM workflows. These users reflect current GenAI adoption and form the base for future agentic AI workflows:
- 100,000 public officers per month using GenAI tools for personal productivity.
- 10,000 public officers building or configuring AI assistants via WOG tools.
- 200 agency teams across ~80 agencies deploying chatbot-enabled systems.
- 6+ WOG platforms enabling AI / chatbot deployment: Pair, AIBots, VICA, GovText, Sentinel, MAESTRO.
The affected parties include citizens, agencies, and the public service, whose sensitive personal, operational, or government information may be exposed if prompts are not properly protected.
## Use Case
Public officers increasingly use GenAI tools for both individual productivity and agency-level AI assistant/chatbot use cases. These workflows often involve free text that contains both explicit PII and more subtle sensitive information. This includes both citizen and agency data.
They encounter the problem at the point of prompting: before text is sent to an LLM, they need to decide whether it is safe enough to use and whether anonymisation will still preserve enough context for a useful response.
In practice, this decision is often skipped. Privacy risk is not visible or salient to users, and users are usually optimising for speed, convenience, and output quality.
## Pain Point
The root problem is that privacy safeguards lose to convenience. Users lack awareness, prioritise speed and output quality, and bypass safeguards when these reduce LLM utility. Organisations also lack visibility and practical ways to enforce safer LLM use.
At the point of prompting, privacy risk is often not visible, not well understood, and not the user’s immediate concern. Some users may not recognise that sending explicit PII, such as names, IDs, contact details, or citizen case details, can create privacy risks for individuals and agencies. Even fewer recognise that sensitive information can still leak without obvious PII, through context that reveals legal exposure, financial vulnerability, medical conditions, employment issues, or agency-sensitive information.
Even when users know anonymisation is recommended, they are usually optimising for speed, convenience, and useful LLM outputs. If safeguards feel cumbersome or remove too much context, users may bypass them altogether.
## Consequence
- Potential exposure of 500M sensitive PIIs per month through GenAI usage, to grow exponentially as GenAI adoption grows across government systems
- Increased risk of PII leakage, policy breaches, and regulatory non-compliance
- Loss of public trust if sensitive citizen or government data is inadvertently exposed
# User Research and Market Analysis
## User Research
Quantitative survey data on this specific risk does not yet exist, for two structural reasons.
- First, low awareness of the problem is itself the core finding; officers who don't perceive a risk won't report one, making conventional demand surveys circular.
- Second, the impact of privacy leakage is inherently difficult to quantify. We do not have access to logs of what officers are actually sending to external LLMs, and the diffuse, unlogged nature of the exposure means that even agencies lack visibility into their own risk surface.
We therefore relied on qualitative discovery from interviews with individual officers, agency teams, and product managers of WOG AI platforms. We also drew on our product management experience with Cloak, which gives us visibility into user needs, adoption barriers, and the types of sensitive information agencies seek to anonymise. 

This problem statement drew most heavily from 10 users:
6 agency users: IRAS, GovTech POD, CareCorner, TRUST, MSF, ESG
5 WOG AI tools: Sentinel, AIBots, GovText, VICA, MAESTRO

Three recurring needs emerged:
1. Better detection of residual sensitive information. Some agencies handle citizen correspondence where sensitive legal, financial, medical, and social circumstances may remain inferable even after obvious PII is removed.
1. Live risk education for officers. Agencies encouraging LLM adoption need officers to make better decisions about whether data is safe to send.
1. Utility-preserving anonymisation. Across Cloak product feedback, users are concerned that anonymisation reduces output quality. They need minimally placeholders that preserve distinctions between entities, and restoration flows that make the final output usable.
## De-risking
- Demand risk: We are not primarily betting on users wanting this today. The hackathon itself is a mechanism to surface the problem to agency leaders and policy teams who set adoption requirements. The Privacy Leakage Score is designed to be demonstrably alarming; showing the gap between what an officer thinks they sent and what an adversarial model can infer.
- Trust / accuracy risk: Implicit inference is inherently probabilistic. We mitigate by being transparent - showing both the score and the reasoning behind it - so officers can exercise judgment rather than blindly trusting the tool.
- Implementation risk: These new features add compute to a flow where users expect speed. If safeguards are slow, users may bypass them. We are de-risking this through parallel work on faster inference for self-hosted models, so the privacy layer can support real-time or near-real-time LLM workflows without becoming a bottleneck.
## Stakeholder Buy-in
- Multiple healthcare stakeholders (MOH TRUST, NHCS, NUHS): These features will be piloted through a Project Agreement with NHCS in 2H26, and if successful be propagated through the healthcare/ research ecosystem through TRUST.
- Social service sector: A coalition of Social Service Agencies representing the top 3 providers of family services in Singapore expressed interest in adopting/ funding these innovations through a tech innovation grant through the Lien foundation.
- Data Program (Cloak): Is the natural home of these new innovations through a direct tech transfer to Cloak, should they prove their value and organisational alignment.
- Data Practice: Will publish these innovations as standards and best practices.
# Solutioning
## Problem-Solution Fit
- Problem-Solution Fit
PromptGuard addresses the privacy-utility gap through a three-part workflow:
- Detect: It identifies both explicit PII and user-defined sensitive attributes that may be inferred from the prompt.
- Explain: It shows a residual privacy leakage score and explains what remains detectable or inferable after sanitisation, helping users understand whether the prompt is safe enough to send.
- Preserve utility: It replaces sensitive entities with meaningful placeholders, maintains consistency across the prompt, and supports restoration in the final output so users can still complete real LLM tasks.
## Functionality
1. User enters or uploads a prompt intended for an LLM workflow.
1. User selects or configures sensitive attributes they care about, such as legal, financial, medical, employment, cybersecurity, policy, or third-party information.
1. The tool detects explicit PII and inferred sensitive information.
1. The user compares the original and sanitised query.
1. The tool shows residual privacy leakage, including explicit risks and implicit risks.
1. The user sends the safer query to the LLM.
1. The final LLM output can be restored with original entity values where appropriate, preserving usability.
## User Experience
Officers interact with a familiar chat-style interface that mirrors how they already use LLM tools. The intent is zero change to their core workflow. Redaction and scoring happen transparently in the background; officers simply see clean, useful output with entities restored, as if they had typed the original prompt directly. For those who want visibility, the Restoration Details modal and Privacy Leakage Score are available on demand - surfacing what was protected and what residual risk remains - without interrupting the primary task.
## User Validation
To be tested next week.
# Impact & Next Steps
## Success Metrics
Number of high-risk prompts made safer before submission =
Number of high-risk prompts meaningfully reduced before submission/ Total number of high-risk prompts detected
 Where “high-risk” is defined where the unsanitised privacy leakage score > threshold.
This tracks both volume and effectiveness.
## Expected Impact
- Short-Term: Raise awareness of LLM privacy leakage and build organisational support for safer LLM use, including clearer policies, platform safeguards, and privacy-preserving workflows.
- Medium-Term: Drive adoption by individual agencies either through publication of standards/ best practices, productionisation in Cloak, or direct pilots with agencies.
- Long-Term: Embed residual-risk assessment and utility-preserving anonymisation into WOG AI tools and workflows.
- Longer-Term: Move beyond individual LLM prompting to future agentic workflows where sensitive data may be retrieved, transformed, and sent across multiple steps.
