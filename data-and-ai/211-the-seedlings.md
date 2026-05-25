---
title: "The Seedlings - OneLineage"
description: "DataHive holds untapped dependency data across 1040 active data requests — DPAs unable to assess change impact and DCAs to triage impact only after."
sidebarTitle: "The Seedlings"
icon: "users"
---

# The Seedlings - OneLineage

| Field | Value |
| --- | --- |
| Requested team | Seedlings |
| Judging group | Final Judging Group 2 |
| Scheduled time | 1:53pm |
| Team number | 211 |
| Category | Data & AI |
| Booth | 9B-22 |
| Project page | [https://build.tech.gov.sg/projects/2026/211](https://build.tech.gov.sg/projects/2026/211) |
| Product link | [https://p01--frontend-stg--8kqf5fttvj58.skmm8r--govpaas.code.run/](https://p01--frontend-stg--8kqf5fttvj58.skmm8r--govpaas.code.run/) |
| Team members | Joyce Teo; Muthu Palaniappan; Siyin Lin; Wellace Leong; Xuan Tu Tran |
| Match status | normalized-the |

## Summary

DataHive holds untapped dependency data across 1040 active data requests — DPAs unable to assess change impact and DCAs to triage impact only after.

## Full Write-Up

# Problem Statement
## Users
The users affected span approximately 39 agencies and ~1,300 active users on DataHive (with ~1040 active data requests and ~380 datasets), operating across two primary roles:
1. DPA* Data Stewards — agency staff responsible for publishing and maintaining datasets on DataHive. They are affected when they need to plan or execute changes to datasets and have no structured way to identify which downstream consumers will be impacted and the scale of impact.
1. DCA* Analysts and Engineers — agency staff who access datasets to power policy decisions, operational systems, or reports. They are affected when upstream changes occur and they have no field-level visibility into whether or how their specific usage is impacted.
*DPA — Data Providing Agency
*DCA — Data Consuming Agency
## Use Case
DPAs and DCAs encounter this problem at two distinct moments:
1. For DPA Data Stewards — performing impact analysis before making a change to the published dataset that is consumed by DCAs: When a DPA plans a change to a dataset (e.g., schema, data definition, refresh frequency, or coverage), they need to identify which downstream DCAs depend on the affected fields and assess the severity of impact before the change is made. Today, DPAs fill in the Change Log details (i.e., Reason for Change, Scope / Impact to Users, Change Summary, and Change Details) on DataHive manually, without any tooling to query the dependency landscape — leaving impact assessment to their own incomplete awareness.
1. For DCA Analysts and Engineers — triaging impact after a change is deployed: When a DPA's Change Log is fulfilled, a broadcast email notification is sent to all active subscribers of the dataset. DCAs then need to determine, on their own, whether the specific fields they depend on are affected and what action is required. There is no field-level targeting in the notification, meaning DCAs cannot tell from the notification alone whether the change is relevant to their usage.
## Pain Point
DataHive already captures the raw material for a complete dependency map: each data request record contains the requesting agency, the dataset accessed, and the specific fields selected. However, this metadata has never been structured into a queryable dependency graph or connected to any impact analysis workflow. As a result:
- DPAs have no mechanism to systematically identify which DCAs depend on a specific dataset or field before making a change [Insight #3]*
- The Change Log form consists of free-text fields with overlapping categories, leading to inconsistent, repetitive entries that obscure rather than clarify impact [Insight #2]*
- Impact assessment in the Change Log is filled manually and based on incomplete, informal awareness of the downstream dependency landscape — not structured data [Insight #2, #3]*
- Change Log notifications are broadcast to all active dataset subscribers after deployment, with no field-level targeting — DCAs have no structured way to determine, from the notification alone, whether or how their specific usage is impacted [Insight #1]*

The root cause is not a lack of data — it is the absence of a tool that connects the dependency information already available in DataHive to the decision-making moments where it is needed most.
*Insights refer to key findings from user research interviews, see User Research section for details.
## Consequence
Without dependency visibility, upstream changes can cascade undetected across agencies at significant cost. In January 2025, IRAS adjusted its tax cycle timing without notifying downstream agencies (i.e., HOMES), causing erroneous means-test results across 22 schemes and 7 agencies — resulting in $9M in incorrect subsidies ($7M excess, ~$2M under). Rectification required urgent system logic changes, multiple rounds of manual re-extractions, and large-scale reprocessing of raw data.

This is not an isolated incident — it reflects a structural gap. DataHive currently manages ~380 datasets and ~1,040 active data requests. As this network grows, the number of potential dependencies increases, and so does the probability and magnitude of such failures. Without a dependency visibility tool, every dataset change carries the latent risk of an undetected, costly cascade — and that risk compounds with every new dataset and agency onboarded onto DataHive.
How might we enable visibility of the existing data requests on DataHive so that DPAs can assess the blast radius of a planned change before making it, and DCA can rapidly triage impact when a change occurs?
# User Research and Market Analysis
## User Research
Method: Qualitative user interviews with DPA Data Stewards and DCA Analysts/Engineers across 4 agencies (CPFB, DOS TC, IRAS, and MyInfo).
Key insights:

1. Notification & Discovery Gaps
- DPAs on DataHive are also DCAs of upstream source agencies — they depend on constituent datasets to derive and publish their own. These DPAs are excluded from upstream planning by source agencies, leaving insufficient lead time to assess impact on their derived datasets, update them, and inform downstream DCAs via Change Logs.
- As DCAs of upstream source agencies, DPAs lack automated early warning — they discover upstream changes only by accident or through routine manual cross-checking. When an anomaly is detected, critical lead time is burned investigating root cause, achieving internal consensus, and seeking management clearance before a Change Log notification can be drafted for their own downstream DCAs.
- One DPA (DOS TC) conducts an annual call-out to all source agencies to solicit upcoming changes — an active but manual workaround in absence of automated alerts.
- Even when changes are communicated, true impact is obscured — DPAs water down language to avoid exposing errors, and automated email notifications use generic titles that resemble spam to DCAs, causing them to be ignored.
2. Change Log Quality & Structure
- Change Log form on DataHive is unstructured (all fields are free-text) with overlapping categories like Reason, Scope, Summary, Details — DPAs end up repeating similar information across fields rather than providing clearer context. DCAs must then read through paragraphs of repetitive content and manually triage impact, shifting the burden of determining what action to take to the consumer.
- DPAs tend to under-represent or over-generalise impact in Change Logs, causing misunderstanding of actual impact by DCAs.
- DPAs struggle to balance messaging for both business and technical audiences in a single Change Log entry.
3. Dependency Awareness & Blast Radius
- DPAs are more interested in the number of affected data requests (to gauge blast radius) than in individual data request owners or team members.
- DPAs want to know the purpose type of affected data requests (e.g., Policy & Planning, Ops & Service Delivery) rather than reading raw justification text.
- A gap exists between what data fields DCAs request and how they actually use them. Views diverge: one DPA (DOS TC) feels strongly that DPAs should provide facts on actual changes and it is the DCA's responsibility to evaluate impact on their own systems; other DPAs (e.g., IRAS) feel this gap requires two-way communication as it is unsustainable for DPAs to bridge alone.
## De-risking
1. Behavioural adoption: DPAs fill Change Log impact details based on incomplete, informal awareness of the downstream landscape — and may under-represent impact to avoid exposing data quality issues.
  - Mitigation: Change Log form replaces free-text with structured guided fields (dropdowns, checkboxes). Impact analysis is computed by the system from the dependency graph, not manually by the DPA.
1. Accuracy of impact assessment: Impact assessment today relies on each DPA's own limited knowledge of the downstream dependency landscape, with no mechanism to query it systematically.
  - Mitigation: Dependency graph surfaces the full downstream landscape. Impact tiering automates severity assessment per data request and field. LLM-powered analysis generates tailored insights for DCAs.
## Stakeholder Buy-in
DPA Data Stewards and DCA Analysts/Engineers from the following 4 agencies participated in user interviews and expressed interest:
- CPFB
- DOS TC
- IRAS
- MyInfo
# Solutioning
## Problem-Solution Fit
[table block omitted in flat markdown; see narrativeBlocks in JSON]
## Functionality
The following diagram depicts the key user flows.
[image](https://wjbbfxaztzhszi7i.public.blob.vercel-storage.com/collab-media/cmnwuahyy006h04ju3taq09as/019e10fe-9fa9-7567-a86f-dbf25acaaba0-User%2520Journey%2520Diagram.png)
## User Experience
1. Dependency UI: Interactive graph visualisation allows users to pan, zoom, and drill down from agency-level to field-level dependencies — no manual cross-referencing needed
1. Change Log form: Structured with guided inputs (dropdowns, checkboxes) to prevent fatigue and ensure consistency — no free-text sprawl
1. Dataset page: Shows active data requests at a glance — users can click into any dataset to see its dependency graph and drill down further
1. Data request page: Shows datasets per DR, type of DR, and status at a glance for all data requests — users can click into each DR to see its dependency UI and drill down for more details
1. Impact tiering: Per-data-request and per-data-field severity labels (High / Medium / Low / None) reduce cognitive load — users immediately know what to focus on
1. LLM-powered analysis: Generates plain-language impact summaries and action steps for each DCA — eliminates manual interpretation of raw change details
## User Validation
User testing with prototype is pending. Feedback will be incorporated post-testing.
# Impact & Next Steps
## Success Metrics
[table block omitted in flat markdown; see narrativeBlocks in JSON]
## Expected Impact
Short-term (immediate upon launch):
- DPAs can run a dependency check before raising a Change Log — replacing informal, off-platform assessment with structured, data-driven visibility
- DCAs receive targeted in-app notifications — reducing noise and containing all change communications within a single platform
Medium-term (with adoption):
- DPAs submit Change Logs with higher confidence that downstream consumers are informed and prepared
- DCAs complete impact triage in minutes instead of days — no manual cross-referencing of change details against their data requests
Long-term (at scale):
- Proactive coordination becomes the norm — both DPAs and DCAs operate with full visibility, eliminating surprise disruptions across the inter-agency data network
- Risk of costly cascading failures (e.g., the $9M IRAS-HOMES incident) is structurally reduced through systematic dependency awareness
Link (https://www.youtube.com/watch?v=p-O3zpBaFro) to OneLineage Demo Video
