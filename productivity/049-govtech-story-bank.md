---
title: "GovTech Story Bank - GovTech Story Seed Bank"
description: "GovTech lacks a central “story bank” to capture and turn product and technical work into reusable marketing content and stakeholder engagement content"
sidebarTitle: "GovTech Story Bank"
icon: "users"
---

# GovTech Story Bank - GovTech Story Seed Bank

| Field | Value |
| --- | --- |
| Requested team | GovTech story bank |
| Judging group | Final Judging Group 4 |
| Scheduled time | 2:03pm |
| Team number | 49 |
| Category | Productivity |
| Booth | 9A-13 |
| Project page | [https://build.tech.gov.sg/projects/2026/49](https://build.tech.gov.sg/projects/2026/49) |
| Product link | [https://story-seedbank.gvt-build26-ideabank.stg.paas.sandbox.gov.sg/](https://story-seedbank.gvt-build26-ideabank.stg.paas.sandbox.gov.sg/) |
| Team members | Anusha Ratnakumar; Jia Hen Tee; Jia Ling Goh; Mark Ng From.businessedge; Ming Fai Wong |

## Summary

GovTech lacks a central “story bank” to capture and turn product and technical work into reusable marketing content and stakeholder engagement content

## Full Write-Up

# Problem Statement
## Users
There are about 50+ story seekers across 3 main teams - external comms (CMG), internal comms (OE), and CIO strategy office (GDT).
- CMG — Marketing external channels include social media, corporate website, and pitches to mainstream media.
- OE Internal Comms — Internal comms channels include GovTech’s monthly newsletter reaching ~4,000 recipients, townhalls, and internal events.
- CIO Strategy Office —
## Use Case
These 50+ seekers across marketing, comms, and strategy teams need to communicate GovTech’s good work and successes for social posts, newsletters, and executive-level decks.
Some external comms channels like social media and corporate website blog operate at a faster cadence of requiring fresh content every week while strategy teams approach marketing on a stakeholder-engagement basis.
Today, finding or landing a single story can require 1–2 months of manual work (based on user interviews): searching Slack channels, cold-emailing product teams, following up via Teams calls, and running face-to-face interviews — sometimes covering ground another seeker already covered. The goal is to discover the story, verify it, and deliver it in the right format for their channel.
## Pain Point
The root cause is not a lack of content, but the lack of a shared system to capture and use it. Without an easy way to discover stories, we miss opportunities to gain greater mindshare and forge collaborations.

Today, product information already exists across decks and documents that teams use to communicate with their immediate stakeholders. 

However, this information is:

Not structured in a consistent way that others can easily understand.
Often too technical or incomplete for non-product teams.

At the same time:

Product teams are focused on delivery and do not have the time or context to translate their work into clear, reusable content. They also have no proof that sharing helps their OKRs. Stories that exist — in standup threads, old decks, and private email inboxes — stay there.
Marketing teams rely on manual requests and repeated back-and-forth to gather and refine inputs.
Product teams are unsure what information is useful to share, and how to present it in a way that helps drive awareness and adoption.

Because there is no shared workflow connecting both sides:

Product teams are unsure what to submit, how to submit, and how marketing teams' efforts can benefit their teams. 
Marketing teams lack visibility into what content exists or is ready to use.

As a result, valuable product knowledge remains scattered and underused, instead of being easily shared, discovered, and turned into content.
 Marketing officers have no central place to look, so every discovery cycle starts from scratch. There is also no agreed-upon "good enough" bar: CIOs like Khoon Hock (SEAB) say they don't know if their story is worth submitting, and the anti-boasting norm makes voluntary contribution feel awkward.
## Consequence
1. Reduced Visibility and Adoption of GovTech Products
- Important products and features remain under-discovered or underutilised because stakeholders and users are unaware of them or do not understand their value.
- Marketing channels become skewed toward the “loudest” teams, while quieter but high-impact products receive little visibility.
- Valuable work gets built but is not sufficiently reused, adopted, or scaled across government. This limits awareness and adoption, reducing the product's overall return on investment.
### 2. Inefficiency and Duplicated Effort
- CMG external comms, OE internal comms, and CIO strategy teams repeatedly approach the same product teams for similar information.
- Around 50 marketing officers and multiple product teams spend significant time chasing updates, clarifying technical details, and recreating content from scratch.
- Stories lose quality and detail as information is reconstructed long after milestone events.
### 3. Slower and More Reactive Marketing Operations
- Without structured, ready-to-use product inputs, marketing teams operate in a reactive, last-minute mode.
- Delays in content production lead to missed launch and announcement windows.
- GovTech becomes slower in responding to leadership, media, and stakeholder requests for impact stories and proof points.
### 4. Reputational and Organisational Impact
- GovTech risks appearing slow or disconnected in communicating its achievements publicly.
- As noted by CMG Social: “It looks like we're slow in conveying information to the public on our official platforms, because it's announced through more personal platforms.”
- Product teams and engineers receive less recognition for their work, reducing opportunities for thought leadership, talent attraction, and internal morale. For the organisation, this reduces opportunities to brand and highlight our good work, demonstrate thought leadership, or drive talent attraction.
# User Research and Market Analysis
## User Research
We synthesised 8 interview inputs (including paired and group interviews) and a 13-response supplier survey across all 4 user groups during Weeks 1–2 of \{build\} 2026 (April 2026), covering external marketing (CMG social, media comms), internal comms (OE), agency stakeholder managers (SPO, CIO teams), and product managers.
Key findings from interviews:
- The unknown story gap is the real problem. Melissa (OE Internal Comms): "There are many good stories around that we don't hear of just because it's not on the Slack channel or not mentioned in the speech." High-profile products are systematically over-represented; quieter teams never surface, regardless of merit. The bottleneck is discovery, not writing quality.
- Cross-team duplication is endemic. OE and CMG independently re-interview the same product teams with no shared transcript or story bank. Janelle (OE) described a desired cross-team workflow: "Between CMG and OE, we could have a workflow — can we work off that transcript first, then send in additional questions?"
- Suppliers need OKR alignment, not better UX. Wen Rui (product manager): story bank contribution is "a nice to have but not a must have" unless it demonstrably helps his team's goals. The Transformation Office product marketing deck — which shows how profiling effort feeds back to adoption metrics and stakeholder visibility — is the closest existing proof point for the incentive model.
- Agency incentive already exists at the leadership level. Ming Hong (LAUNCH/NAIG): agencies want to demonstrate to upper management that AI work reached production. The motivation is real at the organisational level; the platform is missing.
- Serendipitous story depth requires domain knowledge, not just AI. The MOF Budget porridge story (a tradition where the MOF auntie cooks porridge for staff on Budget Day) only emerged because the human interviewer knew to ask. AI chatbot intake must be primed with contextual probes — cultural traditions, behind-the-scenes moments — to approximate this depth.
## De-risking
Using a Lean UX 2x2 matrix, we focused the write-up on two highest-leverage TEST FIRST risk clusters — the ones that most directly decide whether GovTech Story Bank should be built as a repository, an incentive system, or a passive discovery layer:
1. Supply risk: Will product teams actually contribute once a central bank exists? We designed Experiment 1 (DM 5 PMs, ask for a 5-bullet story, no OKR pitch) to measure baseline contribution rate, and Experiment 2 (OKR-pitch variant to non-responders) to test whether aligning submission to team goals shifts the needle. If both fail, the core premise is motivational, not structural — and building a better repository won't solve it.
1. Root cause risk: Is the problem structural (no central repo) or motivational (no reason to share)? Experiment 3 (passive Slack crawl — surface leads to marketing officers) tests whether automated discovery can supply stories without asking product teams at all.
The full matrix also tracks adjacent risks around measurable adoption impact, minimal translation effort, and provider platform fit; these are important, but less decisive for the v0 demo path than supply and root-cause validation.
We also confirmed market demand: rich story raw material already exists in Ming Fai Wong's (SPO Director) own SPO inbox and deck corpus. With his consent and the v0 redaction model, this is sufficient for the demo crawl dataset; wider inbox, Slack, or unreviewed-deck ingestion still requires formal v1 clearance. This confirms that the supply-side gap is not a content gap but a discoverability and governance gap.
## Stakeholder Buy-in
- CMG (Sharleen, Zhengyi, Zoe) — expressed strong interest in a proactive story discovery platform; confirmed that reactive social media caused by late discovery is a live pain point.
- OE Internal Comms (Janelle, Melissa) — confirmed direct relevance to monthly newsletter workflow; requested cross-channel crawling, visibility into prior outputs, and cross-team transcript sharing.
- SPO/GDT Strategy (Ming Fai Wong) — named as sensitivity policy owner for the platform; committed to providing an SPO-owned inbox and deck corpus as the v0 crawl dataset, removing the need for formal data access only for the demo scope.
- NAIG (Ming Hong) — aligned the platform's story quality rubric (Problem / Solution / Outcome / Mouthpiece) with the existing NAIG template, creating a shared bar across seeker groups.
# Solutioning
## Problem-Solution Fit
GovTech Story Bank attacks the discovery gap directly. Instead of asking story suppliers to write, it ingests their existing artefacts — emails, decks, Slack posts, Annual Report submissions — and extracts structured claims. Through an AI-powered chatbot, story seekers can provide prompts to get the results they want and reiterate the results, providing a foundation which they can then bring to product teams to get more information from.
Seekers query once and receive a synthesised story with citations back to the original source, rendered in the channel format they need (tweet, newsletter blurb, CE deck slide, NAIG one-pager). No re-interview required. The incentive loop for suppliers closes through the gap inspector: product managers see exactly which claim is missing from their story page and can plug it by dropping a deck on the flagged field — contribution becomes "plug a hole," not "write a story."
## Functionality
#### Marketing Officer Flow (From perspective of someone who needs a story)
1. CMG officer opens Storybank and queries: "Products that helped agencies save time with AI in 2025, with a willing mouthpiece."
1. The wiki returns matching story pages, each structured as four quality fields: Problem, Solution, Outcome, Mouthpiece.
1. Officer selects a story and clicks "Render as tweet" — receives a draft tweet with claim-level citations.
1. Officer clicks any claim in the draft to drill down to the specific deck slide or email it was extracted from (the trust ladder).
1. The story enters a pre-publish supplier review — the supplier sees the final article and approves before it goes live.
#### Product Manager Flow (From perspective of someone who can provide a product story)
1. PM receives a concierge interview request for product information
1. Answers are ingested as structured claims into the product's wiki page.
1. PM receives a gap notification: the story page is "undersourced" on Outcome. The gap inspector shows the exact field missing.
1. PM drops a deck on the flagged field; the claim updates within 1 minute.
1. PM receives a pre-publish notification before the article goes live — reviews sensitivity, positioning, and quote attribution, then approves.
## User Experience
Three UX decisions make the experience work for both sides of the seeker/supplier dynamic:
- Multi-channel rendering — one wiki page renders as a tweet, a newsletter blurb, a NAIG one-pager, or a CE deck slide without re-extraction. Seekers stop re-interviewing the same team for different channels.
- Drill-down trust ladder — every claim in any rendered output links to the specific source artefact (slide, email, Slack post). Editors can verify without picking up the phone.
- Source-tiered sensitivity model — crawled content is automatically redacted before surfacing: agency names become "Agency A", financial figures become "[REDACTED-$]", PII is removed. Suppliers see exactly what will be published in the pre-publish check, so they trust the pipeline.
## User Validation
The v0 pilot executed an end-to-end demo using the SPO corpus to test our three foundational TEST FIRST hypotheses.
### A. Supply Hypothesis
"PMs will contribute when a central bank exists."
- What Worked: The creation of a centralized repository successfully triggered proactive baseline contributions from Product Managers (PMs) and Delivery Managers (DMs) during the Experiment 1 baseline.
- Areas for Improvement: High friction remains a risk. We are analyzing specific drop-off points to determine if a 5-bullet structured request provides the right balance of context versus user friction.
### B. Root-Cause Hypothesis
"Passive crawl can supply stories without asking PMs."
- What Worked: The passive crawl successfully surfaced net-new story leads from the SPO corpus that had never been discovered by manual seeker interviews. Initial feedback from CMG/OE suggests these leads offer strong foundational material.
- Areas for Improvement: "Missed-context" cases occurred where the AI aggregator over-redacted or stripped away highly specific, humanizing nuances (e.g., the serendipitous MOF "porridge-style" detail). Refinement is needed to balance security redaction with narrative color.
### C. Gap-Inspector Hypothesis
"'Plug a hole' framing lifts contribution rate vs. open-ended asks."
- What Worked: Targeting PMs with explicit, localized gaps (e.g., "Your story is missing an Outcome") yielded a higher response rate across the 3 tested PMs compared to broad, open-ended requests for "updates."
- Areas for Improvement: UX clarity needs tightening. Some PMs experienced latency between receiving a notification and executing the "plug," occasionally struggling to identify exactly which field was flagged for attention.
# Impact & Next Steps
## Success Metrics
### North Star Metric
Time from story creation event to publication-ready channel output — measured in business days.
- Baseline today: 30–60 days (manual hunt + interview + draft)
- Target: under 3 business days
A secondary leading indicator: number of story pages with all 4 quality fields sourced (Problem, Solution, Outcome, Product POC). This measures pipeline health upstream of any seeker query — if the wiki is well-stocked with complete pages, seeker query time approaches zero.
## Expected Impact
#### v0 Pilot — Feedback Bazaar (15 May 2026)
- Demonstrate a full end-to-end flow: crawl ingest → structured wiki page → multi-channel render with drill-down citations, zero re-interviews.
- Validate that passive crawl surfaces stories from quiet teams that seeker interviews missed.
- Test gap inspector with 3 product managers: measure whether "plug a hole" framing increases contribution rate compared to open-ended story requests.
- Target: 5 story pages fully sourced across 4 quality fields from Ming Fai's crawl corpus.
#### v1 — Post-Finale Incubation (July 2026 onwards)
- Onboard CMG, OE, and SPO as active seeker channels, starting with the officers already represented in the interview cohort.
- Expand crawl corpus from Ming Fai's inbox to Annual Report pre-filtered submissions and Slack community channels.
- Implement formal legal clearance for wider crawl ingest.
- Build OKR feedback dashboard so story suppliers see downstream impact — adoption metrics, media reach, stakeholder visibility — closing the incentive loop.
- Target: reduce average story discovery time from 60 days to under 5 days for onboarded seekers.
#### v2–v3 — Long Term
- Self-serve supplier portal: product teams manage their own story pages and track their story's downstream channel performance.
- Cross-GovTech shared transcript layer: eliminate the 4-seeker re-interview duplication entirely.
- Export potential: the Karpathy-pattern LLM-wiki architecture could serve as a reusable model for WOG agencies managing their own story banks (e.g., NAIG agency reports, ministry comms teams).
- If the model proves out, the story bank pattern solves a structural organisational knowledge problem that exists in every large government department — not just GovTech.
