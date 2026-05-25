---
title: "SCOPE - SCOPE"
description: "SCOPE flags capability overlaps between proposals and existing central products, accessible via web portal or as a Claude Code skill."
sidebarTitle: "SCOPE"
icon: "users"
---

# SCOPE - SCOPE

| Field | Value |
| --- | --- |
| Requested team | SCOPE |
| Judging group | Final Judging Group 4 |
| Scheduled time | 2:23pm |
| Team number | 13 |
| Category | Productivity |
| Booth | 10A-03 |
| Project page | [https://build.tech.gov.sg/projects/2026/13](https://build.tech.gov.sg/projects/2026/13) |
| Product link | [https://ui.gvt-build26-scope.prd.paas.sandbox.gov.sg/](https://ui.gvt-build26-scope.prd.paas.sandbox.gov.sg/) |
| Team members | Benedict Ng; Emmanuel Soon; Jiew Peng Lim |

## Summary

SCOPE flags capability overlaps between proposals and existing central products, accessible via web portal or as a Claude Code skill.

## Full Write-Up

[image](https://wjbbfxaztzhszi7i.public.blob.vercel-storage.com/collab-media/cmnwmr8dt000504jo2z0zfnjf/019e01a9-8dea-74fb-a3b2-41b49e4e1a28-image.png)
(Surfacing Capability Overlap and Portfolio Evidence)
# Problem Statement
## Users
Approximately 400* technical and non-technical WOG officers who scope, propose, or build digital products and whose teams are open to using existing central products.
*derived from the share of officers (the large majority in our poll) whose teams consider using central products rather than building by default.
## Use Case
When scoping a new digital product, WOG officers need to determine whether and how well their intended capabilities are already covered by the 80+ existing central products, individually or in combination. The goal is to use or compose what already exists rather than rebuild it, reducing cost and time-to-market.
## Pain Point
Officers cannot answer in reasonable time the question 'is what I'm about to build already covered by something existing?' Today this takes 5+ hours* per product and ~40 hours** for a full proposal needing several products assessed. This excludes further time needed to clarify with central product teams and to have hands-on trials. The default response is to build rather than evaluate.
Senior GovTech leadership has independently named these gaps at the May 2026 townhall, listing overlap, low awareness, composition difficulty, and onboarding friction as among the priority gaps in the central products portfolio. (emphasis, ours)
*based on officer poll
**a full proposal carries voluminous requirements that typically need several products assessed against them
## Consequence
Across ~400 officers and conservative proposal-frequency assumptions, this represents thousands of hours annually in avoidable evaluation effort (see section on user research). Moreover, slow and uncertain assessment leads to building bespoke/new i.e. the path of least resistance*. If unaddressed, the assessment-effort barrier will continue to drive default-to-build behaviour even where central capability exists and adds to the capability overlap that exists across WOG, estimated at S$130M – S$230M annually** (see Annex A for methodology).
SCOPE does not seek to eliminate bespoke builds, many of which are justified; it ensures overlap is visible before the build decision rather than discovered after.
*based on poll, around half of the officers have already built or commissioned a new product rather than use an existing one, at least partly because checking the existing options would have taken too long. Notably, this held even among officers whose teams are otherwise inclined to use central products, which indicates the assessment-effort barrier operates independently of an agency’s disposition toward central products.
**Each such decision risks committing resources to capabilities that already exist elsewhere in WOG. Individually these are defensible calls; in aggregate they accumulate into redundant capability across the portfolio.
# User Research and Market Analysis
## User Research
Our initial approach was a joint-technical and policy solution; helping officers to surface existing central products with an eventual approval gate to ensure that new proposals are first screened for overlaps so that build decisions are informed.
We engaged stakeholders across 3 layers:
1) Interviews with practice and strategy leadership* to confirm the problem space and test whether policy levers were feasible;
- all agreed that capability overlap of products is a real problem
- enforcement, such as mandating the use central products, is not practical

2) Producer-side poll of 14 PMs covering ~16–17 central WOG products to test whether non-use stems from awareness, fit, or integration
- structural absence of a consistent discovery moment (64% said discovery timing “varies too much to say”; only 21% reported agencies encountering their product before a proposal was written);
- dominant non-adoption reason is that agencies prefer to build for control and ownership, not functional gaps**;
- integration and composability are rarely the primary blockers
3) Interview with CDB/IB committee member to understand their main concerns when evaluating proposals;
- use of central products not a priority (more a good to have)
- primary concern is quality of problem framing and root cause identification
These findings led us to review the gating approach. Enforcement was not viable, and committees were not the right intervention point. We refocused on the officers whose teams are already open to using central products, and on the barrier a tool can actually move.
We then polled 20 technical and non-technical officers;
- the large majority (86%) consider central products
- 100% find it difficult to evaluate whether existing products meet their needs
- most (82%) spend 5 or more hours assessing a single central product; where 50% spends more than 10 hours
- Around 64% have built or commissioned a new product rather than use central products, at least partly because the assessment would have taken too long
That officers near-universally find evaluation difficult is itself evidence of a market gap: current discovery and evaluation methods are not sufficient, which is the gap SCOPE exists to fill.
*including DCE Sau Sheong, ACE/CIO Dominic, ACE Bee Teck, PMP Lead Jona and Developer Portal team, Product Strategy Office officers
**corroborated by PSO's poll of agencies where lack of awareness and fit-for-use did not show up as primary reasons for non-adoption. These refine, rather than undermine, SCOPE's role: discovery alone is insufficient. SCOPE's value is giving officers who do want to use central products the evidence base to win the build-vs-use argument internally. It is the artefact that lets a team make the case against a default-to-build posture, with capability matches the officer can verify rather than assert.
## De-risking
The primary risk is technical: whether SCOPE’s matching engine returns relevant, accurate overlaps on real WOG inputs. If accuracy is poor, officers will not trust it. We ran a limited launch of the working prototype to a separate group of around 20 officers, then polled 10 of them (a mix of technical and non-technical users)
- 100% rated SCOPE's recommendation accuracy high/very high
The secondary risk is demand: evidence needed that there's demand and that officers would actually use SCOPE, not merely say they would.
- 100% of officers polled indicated that a tool surfacing overlapping central products would be useful to their team.
- A limited launch logged >100 uses within the first 2 weeks (use is anonymous by design, with no login required, to keep friction low, so usage is counted but not attributed to individuals).
Other risks
- ownership: without a formal owner, SCOPE risks remaining at prototype stage despite validated demand.
  - Mitigation: post-hackathon, the validated prototype is the artefact that earns the ownership conversation with PSO or TMO. Active engagement is in place with both.
- data: SCOPE's knowledge base is based on data from the developer portal, product scorecard, product catalogue and product team's documentations - these in turn depend on product teams updating the information regularly and reliably.
  - Mitigation: this is a known problem today within the current portal teams which is being reviewed - SCOPE intends to participate in these discussions.
## Stakeholder Buy-in
SCOPE has two candidate owners (PSO and TMO), with active engagement on both sides. The decision to validate the prototype before pursuing formal ownership is deliberate: SCOPE's fit with PSO (problem-statement quality and proposal evaluation) differs from its fit with TMO (catalogue and product-discovery), and the validated prototype is the artefact that lets us have an informed conversation about which home is right. The post-hackathon ask is to convert one engagement into formal ownership within 4-8 weeks.
# Solutioning
## Problem-Solution Fit
SCOPE sharply reduces time needed to evaluate suitable central products based on a submitted proposal to minutes.
Proposals are matched against the WOG product catalogue at the level of capability (beyond product name or owning agency), returning direct matches, partial matches, and combinations of products that together meet the stated need (see Annex B for how SCOPE works).
Teams can decide whether to take it further with the respective product teams or review their build strategy.
Why this approach over alternatives: We considered three approaches:
(a) extending the existing product catalogue/scorecard with better search;
(b) a policy gate at the funding committee level;
(c) an officer-side overlap detection tool.
(a) was rejected because the bottleneck is not merely catalogue navigation but capability-level evaluation effort - better search of the same content does not change the 5-hour evaluation time. Discovery isn't enough; we need to make adoption easy (b) was rejected as politically unviable; our stakeholder interviews surfaced that enforcement would face resistance and risk pushing build activity outside formal channels. (c) is what SCOPE is - it intervenes where the assessment cost actually lands, with the officer making the build-vs-use decision rather than a committee gating it.
## Functionality
Non-technical user (web portal)
1) Uploads a proposal document or types a free-form question into the SCOPE web portal.
2) Reviews the returned list of overlapping and partially-overlapping products, with the matched capability dimensions shown for each.
Technical user (within Claude Code)
1) While scoping or prompting a build in Claude Code, invokes the SCOPE skill, with no switch to a separate portal.
2) SCOPE returns overlapping and partially-overlapping central products inline, in the same workflow, before any build is committed.
3) Reviews the matches and decides whether to use and/or compose central products, or proceed with the build.
## User Experience
For non-technical users familiar with navigating portals, SCOPE accepts free-form input (a proposal in PDF or Word, or a free-form question) and returns an evidence-linked list. There is no new interface to learn beyond describing what you are trying to build.
For technical users who natively use Claude Code to build, SCOPE is available as a skill. This matters as requiring this group to toggle between a portal UI and Claude Code would introduce friction and sit outside their workflow. The skill brings overlap detection to where they already work.
## User Validation
From the 10-officer prototype poll (the same cohort drawn from the limited launch): 100% agreed that SCOPE saved them time; 90%* said they would be more likely to consider central products because of SCOPE.
*the one dissenting respondent cited senior leadership's posture toward central products
Selected qualitative feedback
"Pretty good analysis....exactly what we are currently doing, tapping on App A* to plug the gaps on App B* e.g. send alerts to agencies which have yet to provide outcome after 'X' days....which currently App B* is unable to support."
"It is good because the suggestions it gave me allowed me to know what products out there, and whether they can or cannot fit my use case."
"looking forward to seeing this live. it will save me a lot of pain as a first cut for assessment."
*intentionally anonymised
# Impact & Next Steps
## Success Metrics
North Star: % of WOG digital-product proposals that include documented consideration of central products in their solutioning.
This is the system-level outcome SCOPE exists to move: from a baseline today where many proposals do not consider central products at all, to a future where consideration is the documented norm. SCOPE's contribution is to make consideration cheap enough to be expected, ahead of any formal requirement to document it. The metric is not yet directly measurable across WOG, which is itself a gap a future SCOPE deployment can help close.
Leading indicators:
- Usage rate: >30% of officers reached use SCOPE within one month of launch
- Accuracy: >85% of users rate recommendation accuracy “high” or “very high” within one month of launch
- >25 Claude Code skill downloads

Lagging indicators:
- >20% uplift in officer-initiated queries to central product teams (for products SCOPE surfaced), with 20% of those queries converting into use or composition outcome, measured over 12 months
- A rising trend in the % of users reporting that SCOPE increased their awareness of central products
- Increasing breadth of adoption: the number of GDT-agencies whose officers have invoked SCOPE at least once per quarter
## Expected Impact
Short term (0–6 months post-hackathon): A working prototype with measured matching performance on real WOG inputs. Identification of an owner for SCOPE (PSO/Innovation Office, TMO, or another office best positioned to house it), and higher adoption through direct officer outreach. Refinement of SCOPE’s knowledge-base indexing and routines.

Medium term (6–18 months): Collaboration with agency CIOs and the practice families (Engineering, Product, Design, Business Analysis, Project Management) to raise visibility and adoption through their endorsement. A smoother hand-off between an officer acting on a SCOPE result and the relevant central product team.

Two dependencies govern the roadmap: (i) an owner for SCOPE is identified, with the validated prototype as the artefact that earns this conversation and active engagements summarised under Stakeholder Buy-in; (ii) the WOG product catalogue is sufficiently indexed and kept current, a known dependency on TMO’s existing catalogue work. Detection reliability is handled by design: SCOPE surfaces evidence and links to the underlying matches, and never asserts a verdict.
## Annex

The annexes preserve supporting detail for readers who want the underlying material. Nothing in the main writeup depends on these for completeness; they are reference material.
### 
Annex A. Cost Estimation Methodology

Singapore illustrative estimate S$130M – S$230M annually: Singapore Government FY24 ICT spend is approximately S$3.3 billion[3]. The range above represents what 4–7% of this spend going toward capabilities that overlap with what already exists would amount to, anchored on the UK State of Digital Government Review’s 4–7% broader digitisation-savings estimate for the UK public sector[2]. The figure is illustrative, not measured.

Method and caveats: we do not have a Singapore-specific benchmark for capability overlap as a percentage of ICT spend. The 4–7% range used here is taken from the UK State of Digital Government Review’s broader digitisation-savings estimate for the UK public sector [2], applied to Singapore’s FY24 ICT spend. This is an analogue rather than a derivation: the UK figure spans broader digitisation savings rather than capability overlap specifically, but it is the nearest government-grade reference point available. We treat the 4–7% range as conservative-to-plausible pending direct measurement, and readers should apply their own judgement on whether it is appropriate for the WOG context. The range is intended to convey order of magnitude, not precision.

Government precedents support the order of magnitude: the US GAO has documented approximately US$725 billion in financial benefits from 2011 to 2025 by addressing fragmentation, overlap, and duplication across the federal government[1]; a single recommendation in their 2025 annual report on IT portfolio reviews was assessed as capable of generating US$100M+ on its own. The UK’s 2025 State of Digital Government Review identified fragmentation and duplication as systemic (44 different ways to prove identity to government in 2021), with broader digitisation savings estimated at £45 billion per year, or 4–7% of total UK public sector spend[2]. These are not direct analogues for capability overlap in WOG ICT spend specifically, but they show that the structural conditions producing material avoidable costs are well-documented in comparable governments.

The absence of any systematic measurement of capability overlap cost in Singapore is itself part of the problem SCOPE addresses. A medium-term outcome of SCOPE adoption is the data needed to replace this estimate with a measured figure.
## References

[1] U.S. Government Accountability Office (2025). 2025 Annual Report: Opportunities to Reduce Fragmentation, Overlap, and Duplication (GAO-25-107604), 13 May 2025. https://www.gao.gov/products/gao-25-107604
 (https://www.gao.gov/products/gao-25-107604)[2] UK Department for Science, Innovation and Technology (2025). State of Digital Government Review, 21 January 2025. https://www.gov.uk/government/publications/state-of-digital-government-review/state-of-digital-government-review
 (https://www.gov.uk/government/publications/state-of-digital-government-review/state-of-digital-government-review)[3] GovTech Singapore (2024). “FY24: Government to spend more than $3B to modernise ICT infrastructure and develop digital services”. https://www.tech.gov.sg/media/media-releases/fy24-government-to-spend-more-than-3b-on-infrastructure-and-digital-services/
### Annex B. How SCOPE works
SCOPE parses the proposal or query into discrete capability claims, then matches each claim against the indexed WOG catalogue at the capability level, using a combination of keyword, semantic, and hybrid search. An agent compares what the proposed build seeks to do against what existing products already do, and returns direct matches, partial matches, and multi-product combinations, each linked to the underlying capability evidence so the officer can verify the result rather than take it on trust.
SCOPE's knowledge base is currently based on products in the developer portal, product scorecard and product portal.
