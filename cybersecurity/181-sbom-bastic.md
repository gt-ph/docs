---
title: "SBOM-bastic! - Dependency Map"
description: "A unified visibility platform that enables security teams to quickly identify affected systems, components, and owners during cyber incidents."
sidebarTitle: "SBOM-bastic!"
icon: "users"
---

# SBOM-bastic! - Dependency Map

| Field | Value |
| --- | --- |
| Requested team | Sbom-bastic |
| Judging group | Final Judging Group 3 |
| Scheduled time | 2:13pm |
| Team number | 181 |
| Category | Cybersecurity |
| Booth | 8B-09 |
| Project page | [https://build.tech.gov.sg/projects/2026/181](https://build.tech.gov.sg/projects/2026/181) |
| Product link | [https://idependonwhat.cio.sandbox.gov.sg/](https://idependonwhat.cio.sandbox.gov.sg/) |
| Team members | Ahmad Zahiri; Aloysius Wang; Amalina Rashid From.scientec; Danial; Muhammad Al-Fairuz |

## Summary

A unified visibility platform that enables security teams to quickly identify affected systems, components, and owners during cyber incidents.

## Full Write-Up

# Problem Statement
## Users
Incident responders, agency security teams, and system owners across Whole-of-Government (WOG)
## Use Case
When a new cyber threat emerges (e.g. vulnerable npm package or supply chain attack), incident responders must quickly determine which systems are affected and who owns them, often within the first few hours and before formal advisories are released, to initiate response plans and coordinate remediation.
## Pain Point
Responders spend hours manually checking multiple tools, systems, and stakeholders to identify affected systems. Dependency and ownership data are fragmented, and visibility into indirect (transitive) dependencies is limited, making impact assessment slow and inconsistent.
## Consequence
A large portion of the response window is spent on impact identification, delaying containment and increasing the risk of exposure across multiple systems and agencies.
# User Research and Market Analysis
## User Research
Conducted interviews with 5 stakeholders, including incident responders, MCISOs, and agency security teams involved in incident response.
Synthesised insights from real incident workflows and recent scenarios (e.g. axios supply chain vulnerability) to understand how teams identify affected systems and coordinate response.
Key findings:
1. All participants reported having to rely on multiple tools and sources (e.g. CodeSCAPE, SHIP-HATS team, etc. ) to determine affected systems
1. 100% of participants identified determining affected systems as the most time-consuming step during incident response
1. System ownership is not centrally visible, requiring manual coordination across teams
1. Teams have low confidence in coverage completeness, especially for indirect dependencies
## De-risking
1. Data Fragmentation & Coverage Risk
  Dependency, ownership, and system data may be fragmented, incomplete, or outdated, limiting accurate impact identification and reducing trust in the platform. All participants reported relying on multiple tools during incidents, confirming that data exists but is not unified.
  We mitigate this by starting with higher-coverage data sources (e.g. systems on AWS environments) to deliver immediate value, while designing the product to correlate fragmented data through DGP id. The product is also built to support future integration with live data sources to improve freshness and coverage over time.
1. Workflow Adoption Risk
  Incident responders work under time pressure and may not adopt a new platform if it adds friction to an already stressful workflow.
  We mitigate this by designing around the earliest and most painful step of incident response i.e. identifying affected systems and ownership, with a single search entry point and ownership information surfaced alongside dependency data, reducing the number of tools a responder needs to consult rather than adding to them.
1. Scope & Focus Risk
  The problem space is broad and risks producing an unfocused solution.
  We mitigate this by anchoring all product decisions to a single use case i.e. rapid identification of affected systems and ownership during a cyber incident. Features that do not directly reduce time to identify affected systems and ownership are intentionally deferred, keeping the product focused and avoiding scope creep into general asset management.
## Stakeholder Buy-in
GITSIR and GCC
# Solutioning
## Problem-Solution Fit
Dependency Map directly addresses each validated pain point:
1. Fragmented tooling > Unified search and view
 A single platform allows responders to search across systems, components (e.g. packages, software), and hosting environments, aggregating dependency and ownership data into one place and eliminating the need to consult multiple tools during an incident.
1. Slow identification of affected systems > Rapid dependency mapping
 Searching a component (e.g. a vulnerable package) instantly surfaces affected systems across agencies, including direct and indirect dependencies, significantly reducing identification time.
1. Lack of ownership visibility > Immediate ownership context
 System ownership is surfaced alongside dependency data, enabling responders to quickly identify and engage the right teams without manual coordination.
1. Low confidence in coverage > Transparent impact visibility
 Interactive dependency graphs and structured views across systems, components, and hosting environments provide clear visibility into relationships and impact, helping teams understand what is known and where gaps may exist.
## Functionality
1. Search and identify affected systems
  - Responder enters a query (e.g. vulnerable package or service such as CrowdStrike) into the search bar
  - The platform returns related systems, components, and hosting environments across agencies
  - The responder views affected systems and their relationships through an interactive dependency graph
1. Determine ownership and initiate response
  - Responder selects an affected system from the results or graph
  - The platform surfaces ownership information (ministry, agency, system owner) alongside dependency data
  - The responder identifies the responsible team and initiates coordination
1. Understand impact through dependency mapping
  - Responder explores direct and indirect dependencies of the selected system or component
  - The platform visualises how the issue propagates across systems
  - The responder reviews impact summaries to assess scope and prioritise response
1. Drill down into system and component details
  - Responder navigates to detailed views of systems, components, or hosting environments
  - The platform provides inventory data (e.g. SBOM, dependencies) and contextual information
  - The responder uses this to support investigation and remediation decisions
## User Experience
Incident response is time-critical, so the experience is designed to get responders to answers as fast as possible with minimal friction.
We prioritise the following:
- Single search entry point
 Responders can start with what they already know, such as a package name, service, or CVE, without needing to navigate across systems or understand how the platform is structured.
- Prioritised information display
 Information is structured to surface the most critical details first, such as affected systems and ownership, allowing users to quickly understand what action to take without deep investigation.
Progressive disclosure of complexity
 Complex dependency relationships are presented in a way that allows responders to see a high-level view first and drill down into details only when needed, avoiding information overload during critical moments.
## User Validation
We validated the solution direction with incident responders and agency security teams involved in vulnerability investigations and incident response workflows.
Feedback consistently highlighted the need for more centralised visibility during active incidents, especially when responders need to quickly determine affected systems, ownership, and potential blast radius across agencies. Users shared that current investigations often require correlating information across multiple fragmented tools and data sources, making impact assessment time-consuming and operationally challenging.
Responders also emphasised that completeness and accuracy of dependency and ownership data are critical, particularly when responding to leadership and management queries during incidents. Teams need to confidently answer questions such as whether they are affected, which systems are impacted, and who needs to take action, often under significant time pressure.
The dependency visualisation was positively received as it helped users better understand relationships between components, systems, and agencies during triage. Users also highlighted that investigation priorities can differ depending on the type of threat or exposure, reinforcing the need for flexible and comprehensive visibility during incident response.
# Impact & Next Steps
## Success Metrics
Time to identify affected systems and ownership
 The time from a threat being identified to a confirmed list of affected systems and owners being available to the incident response team. The goal is to reduce this from hours to under 15 minutes.
Secondary metrics:
- Coverage completeness rate (% of systems with mapped dependencies and ownership)
- Reduction in number of tools consulted per incident
- Responder confidence score (self-reported certainty in completeness of identified impact)
## Expected Impact
We plan to onboard incident responders for a pilot, with the goal of reducing time to identify affected systems and ownership from hours to under 15 minutes during the initial response window.
This is expected to reduce manual investigation effort and reliance on multiple tools, allowing responders to focus on containment and remediation earlier in the incident.
