---
title: "Crunch - Ruru"
description: "Ruru is a local-first hub on COMET that turns 5–10 hours of weekly mechanical work into one-click tools, built in under an hour."
sidebarTitle: "Crunch"
icon: "users"
---

# Crunch - Ruru

| Field | Value |
| --- | --- |
| Requested team | Crunch |
| Judging group | Final Judging Group 2 |
| Scheduled time | 1:30pm |
| Team number | 42 |
| Category | Productivity |
| Booth | 9B-03 |
| Project page | [https://build.tech.gov.sg/projects/2026/42](https://build.tech.gov.sg/projects/2026/42) |
| Product link | [https://crunch-hub.cio.sandbox.gov.sg/](https://crunch-hub.cio.sandbox.gov.sg/) |
| Team members | Edmonds Dale Emily; Jia Liang Sim; Yi Zhen Yao |

## Summary

Ruru is a local-first hub on COMET that turns 5–10 hours of weekly mechanical work into one-click tools, built in under an hour.

## Full Write-Up

# Problem Statement
## Users
Approx 79,000 government officers across WOG with COMET laptops (est. from # of gov. orgs)
## Use Case
Each week, government officers manually fill templates for incident reports, service requests, compliance submissions and stakeholder updates. The same data is re-keyed across multiple formats because every agency has its own forms, formatting rules, legacy systems and standards. The result is repetitive, mechanical work that no commercial or whole-of-government tool covers economically as variation per agency is too high and the user base for any single workflow is too small.
## Pain Point
Government security constraints block the tools that would normally solve this. Cloud automation platforms cannot touch sensitive data. Approved SaaS procurement takes months to years. The systems being managed are legacy or heavily customised and thus often too specialised for any horizontal WOG platform to ever cover.
Meanwhile, the raw capability to automate already exists on every COMET: Anaconda Python, COM automation, an approved browser with GovTech AI access. A dedicated officer with time and persistence can hack together a working solution. But with a framework that handles security, packaging, distribution and AI-guided code generation, the same outcome moves from a multi-week climb to a one-hour build.
## Consequence
Without intervention: compliance jobs go silently overdue because tracking depends on memory. Documents contain copy-paste errors because the same data is re-entered into three formats. Follow-ups fall through. Skilled staff spend 5–10 hours per week per officer on mechanical work that a local Python script behind a web form could eliminate.
# User Research and Market Analysis
## User Research
Research came from four overlapping layers.
Direct observation inside our own agency. The three team members are BAs who actively wanted more automation. The initial module set came from a personal audit of repetitive tasks: manual CAM reviews, Zendesk stakeholder reports, PDF ticket mailing, SSL cert management. The lead builder's own observed productivity gain is approximately 60 hours/month, used as the upper anchor for the power-user tier in the financial model — the model itself holds a more conservative 45 hours/month at that tier.
Informal interviews with peer BA/PMs across neighbouring teams. Unstructured 15–30 minute conversations focused on a single question: what's the most mechanical part of your week that you'd hand off if you could. Recurring answers — privileged user audits, SLA report assembly, stakeholder update drafting, ticket triage — drove additional prototype modules including the checkpoint calendar, inbox triage and SOP flowcharting.
Agency-internal survey of ~100 business users on vibe coding and appetite for small custom solutions on COMET. Results were strongly positive: users want narrow, task-specific tools without going through a lengthy procurement cycle or waiting for ICTD resources, and accept a Python-on-laptop delivery model when the alternative is "wait another six-to-twelve months or do it by hand." This was especially true for problems affecting 1–5 users — too low a priority for full ICTD engagement. Survey results validated the user-tier assumptions in the financial model (10% power / 30% active / 60% light).
Academic literature review to check the citizen-developer / low-code thesis against peer-reviewed evidence (market research is heavily biased towards positivity):
- Ajimati, Carroll & Maher (2025), Journal of Systems and Software. DOI: 10.1016/j.jss.2024.112300. Systematic review of 40 primary studies (2017–2023) on LCNC adoption. Establishes the field is academically active and that adoption barriers, not capability gaps, are the dominant concern — which is what Ruru's packaging architecture targets.
- Bock & Frank (2021), MODELS-C. DOI: 10.1109/MODELS-C53483.2021.00016. Critical exploratory study of seven low-code platforms. Concludes that few individual LCNC features are genuinely novel — value comes from packaging existing capabilities for a non-developer audience. Reinforces Ruru's positioning as a distribution layer for capabilities already present on every COMET, not a new automation technology.

We have also implemented anonymised telemetry into Ruru for incoming beta users to summarise build requests and code patterns, so we can track the problems and solutions users actually pursue.
Key insight 1: The bottleneck is not "users can't automate." It is the absence of a packaging and distribution layer that lets one officer's automation become another officer's installable module under government security constraints. Ruru exists to solve the distribution gap, not just the automation gap.
Key insight 2: most ICTD effort goes to the largest problems; Ruru deliberately inverts this, targeting the long tail of small problems where the affected user count is too small to justify a full ICTD engagement but the aggregate time loss is enormous.
## De-risking
An approved WOG platform overtakes us. GovTech could mandate a centralised RPA or low-code platform that supersedes Ruru. Mitigation: Ruru is positioned as the layer that fills the gap below WOG platforms — agency-specific, system-specific workflows (D365, Zendesk, Amazon Connect) that are too niche for a horizontal platform to ever cover economically. If a WOG RPA platform lands tomorrow, Ruru remains useful for the long tail.
Security review blocks adoption. Local-first execution was a design constraint from day one. The only outbound traffic is a narrowly-scoped call to a GCC-hosted VPS that handles GovTech AI calls and runs sandboxed Python libraries that cannot be installed directly on COMET. Data classification is checked on every egress and ingress, API keys are scoped per officer and wiped after use, and a central audit log captures everything. The architecture is explicitly compatible with the Menlo allowlist regime and supports granular ICTD/agency scoping.
Maintenance burden on a single author/team. Module isolation is enforced by the hub-and-spokes architecture: each module is a self-contained folder, installable as a zip, with no cross-module imports. New contributors only need to understand their own module plus a small shared library. The build_recipe.json schema and ruru-check skill let a non-author validate a module without reading its full source.
## Stakeholder Buy-in
Ruru is in active discussion with our agency's AI team to continue as a funded product beyond the prototype stage. Two factors are driving that conversation: strong user demand from the initial prototype, and very low PoC cost — no new infrastructure, no SaaS licensing, runs on existing COMET laptops with existing approved tooling.
No formal cross-agency commitments yet, but the foundations are in place: the ~100-user internal survey showing strong appetite, informal conversations with BA/PMs in adjacent agencies confirming the same pain points, and a costed three-year financial impact assessment that lets sponsors stress-test the case rather than asking them to accept it.
The path to wider buy-in has two prongs. First, the 25-module finale: a hub home page showing 25 ready-to-install modules covering the most common BA/PM workflows, so adoption is a one-page decision for another agency's IT and BA leads rather than a custom build per agency. Second, treating the agency AI team conversation as the lead reference site — if Ruru lands as a funded product internally, that becomes the proof point for the next agency conversation.
# Solutioning
## Problem-Solution Fit
Each constraint maps to a specific design choice.
No pip install, no admin rights. Ruru ships as a single folder run against the system Anaconda Python already present on every COMET. No installer, no elevation, no DLL registration.
No external APIs on COMET. Modules use COM automation for Word/Excel/Outlook/PowerPoint, the local browser via Playwright where the target system has no API, and local file system access. The only outbound calls go to a GCC-hosted VPS that handles GovTech AI calls and runs a sandboxed Python library service for libraries that cannot be installed on COMET. Data classification is checked on every egress and ingress; API keys are officer-scoped and wiped after use; the VPS holds a central audit log. Multiple rounds of security checks in the build pipeline prevent accidental or intentional data leakage, deletion, or spam.
Behind Menlo. Outbound traffic is whitelist-compatible and the allowlist is documented for IT review.
Re-keying the same data into multiple formats. The hub treats data as the primary artefact. A single incident captured once is rendered into a Word report, two email drafts, and a tracker update by the same module invocation — eliminating the re-keying step entirely.
Tasks going unseen. Modules like checkpoint_calendar and ssl_cert_manager treat the recurring task as state: each run records what was done, what's outstanding, and when the next checkpoint is due, so chasing happens against a list rather than memory.
## Functionality
Ruru is a local web app. The user opens http://localhost in their browser, sees a hub home page of installed modules (either chosen by their agency or self-built), and clicks into the one they need. Each module is a self-contained tile with its own form-driven UI.
Representative flows from the current build:
Incident report: User fills a single form. The module generates a Word incident report, drafts the stakeholder email, and updates the incident tracker, all from one input, customised to their agency's needs.
Zendesk reporter: User pastes or uploads a Zendesk export. The module instantly assembles a block-based report template with charts and an Excel attachment, ready to send. Templates are reusable across reporting cycles, customisable to different stakeholders.
Compliance modules: SSL cert manager, Zendesk access manager, and privileged user audits — monthly flows that parse vendor exports, extract rows needing action, and produce the filed artefact with correct naming and enforcing checks by officer to verify.
Across all modules, the shared pattern is: form input → deterministic Python → AI interaction routed through the VPS where needed → COM/browser/file output → audit log.
## User Experience
Three deliberate choices kept the experience light:
Browser-native UI, no install. Users already know how to open a browser. There is no separate desktop app to learn or maintain. The hub looks like an intranet page.
One module = one screen. Every module fits the same shell: a left rail describing what the module does, a centre column with the form, an output preview on the right. No nested menus, no settings buried two clicks deep. The UI/UX design is enforced across modules for simple and clear design and patterns.
Failure is visible and communicative, not silent. When a module fails — vendor export schema changed, file open in Excel, network blip — the error surfaces in the same panel with a plain-English message and a "what to try" suggestion. The audit log makes it easy to ask "what happened last Tuesday."
A multi-turn AI chat (Converse) is being introduced for new module commissioning, so a user can describe their requirement in conversation rather than filling a structured form.
## User Validation
What worked: Time-to-value is immediate. The first time a PM runs zendesk_reporter on their own export, they get a finished report in seconds — the "this is real" moment happens on first use, not after onboarding. The hub model is intuitive: users grasped "modules are installable apps inside the hub" without explanation. COM-generated Word and Excel files look hand-made, so downstream recipients cannot tell they were generated.
What needed improvement: Early modules required too much per-agency configuration (file paths, template locations). The config.php-style pattern and build_recipe.json schema were introduced specifically to fix this. The first UI generation was inconsistent across modules; the components.css / tokens.css design system and the clean-html-crunchhub audit skill were built to enforce visual consistency without slowing module development. We also added more scoping — explicit lists of what we can and cannot build, plus alternatives — so the AI can coach a possible module into spec rather than failing silently. Some modules (zendesk_reporter) needed a preview-before-send step rather than direct generation; that is now standard for any module producing an outbound artefact.
The end-to-end build pipeline now runs user-designed scenarios through a recipe.json structure, generates components into a framework template, performs contract reconciliation, debug rounds and critic passes across multiple AI models, and uses heavy caching — cutting code generation cost from ~S$25 to ~S$3 per run. A Playwright-managed user testing session at the end validates and smoke-tests the module through a guided session with the user.
# Impact & Next Steps
## Success Metrics
North Star: monthly active users among addressable officers.
Tracked because it is the single metric that compounds everything else. Hours saved, dollar value, and module library reuse all derive from active user count multiplied by per-user engagement. MAU (not installs) is the right denominator: the gap between installs and actives is typically 3–5× for opt-in tools, and only actives generate value.
The Year 1 commit-line is 10% adoption of ~79,000 addressable officers (≈ 7,900 MAU by month 12). Conservative floor is 5%; optimistic stretch is 20%.
Secondary metrics: hours saved per active user per month (validated by sample time-tracking on power users in Q1), modules in active use (library breadth), and overdue compliance task rate (operational impact proxy).
## Expected Impact
Modelled across three scenarios with explicit assumptions on adoption ramp, per-user hours saved, library compounding, and realisation rate. All figures undiscounted; NPV at 5% reduces Y2/Y3 totals by ~7%.
Even under the conservative floor — slow viral spread, modest per-user gains, heavy discounting of self-reported hours — the three-year case is 2.1M hours saved (≈1,036 FTE-equivalent), S$27M net value, and 22× ROI against an S$1.8M programme cost. This is the figure the case stands on.
The base case projects 7.6M hours saved (≈3,787 FTE-years, or roughly 1,260 FTE per year by Year 3 — about 1.6% of the addressable workforce), S$188M net value, 104× ROI.
The optimistic stretch (strong viral spread, mature library producing significant Y3 multipliers, high confidence in dollar conversion) projects 23.9M hours, ≈11,945 FTE-equivalent, S$851M net, 319× ROI.
Programme cost in all scenarios is dominated by AI inference per active user plus ICTD low-code review time; no new infrastructure or licensing.
By time horizon (base case):
Short term (Year 1). ~515k hours saved, S$12.6M net value. Internal pilot expands into the full BA/PM cohort and beyond. The 25-module home page ships. Time-tracking instrumentation on sample power users validates the realisation-rate assumption.
Medium term (Year 2). ~2.2M hours, S$55M net. Library compounding starts to bite (assumed 30% Y2 uplift from reused modules). Two to three adjacent agencies adopt with their own module mix. Cross-agency module sharing becomes routine via the packaging tooling (ruru-package, build_recipe.json, capabilities registry).
Long term (Year 3). ~4.8M hours, S$120M net. Ruru becomes the default answer for "this workflow is too niche for a WOG platform but too repetitive to do by hand." The model generalises beyond BA/PM work into other Comet-bound roles (security, finance, compliance) facing the same constraint stack. Aggregate impact at WOG scale runs into hundreds of person-hours per month redirected from mechanical work to judgement work, with no uncontrolled data egress — all outbound calls are classified, logged, and key-scoped per officer.
