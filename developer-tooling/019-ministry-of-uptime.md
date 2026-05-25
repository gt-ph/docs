---
title: "Ministry of Uptime - AgentOps"
description: "AgentOps is the AI agent platform powering autonomous flow across every stage of the SDLC with human-in-the-loop approvals."
sidebarTitle: "Ministry of Uptime"
icon: "users"
---

# Ministry of Uptime - AgentOps

| Field | Value |
| --- | --- |
| Requested team | Ministry of Uptime |
| Judging group | Final Judging Group 4 |
| Scheduled time | 1:10pm |
| Team number | 19 |
| Category | Developer Tooling |
| Booth | 9E-11 |
| Project page | [https://build.tech.gov.sg/projects/2026/19](https://build.tech.gov.sg/projects/2026/19) |
| Team members | Delon Wong; Jermyn Tanu; Melvin Loo; Ren Fa Kay; Ryan Zhuang |

## Summary

AgentOps is the AI agent platform powering autonomous flow across every stage of the SDLC with human-in-the-loop approvals.

## Full Write-Up

# Problem Statement
## Users
Engineers of different roles across that need to ship new products and keep existing systems reliable at the same time.
## Use Case
The challenge is that engineering teams are trying to keep software changes safe and reliable across the development cycle, but they face too many repetitive operational tasks, fragmented workflows, and hard-to-govern decisions when things fail or need approval. They need to detect issues, validate releases, coordinate remediation, and document outcomes quickly, while still maintaining human oversight for risky action
## Pain Point
Engineering teams often detect issues too late because they rely on manual checks, on-call reactions, and fragmented signals instead of continuous monitoring, so problems can sit unnoticed until users are already affected. This makes detection slow, inconsistent, and dependent on who happens to be watching at the moment.
## Consequence
If the problem is not solved, issues will keep being detected late, so incidents can grow from small anomalies into major outages before anyone responds. That means users experience longer downtime, slower fixes, and more failed releases reaching production, which directly harms trust and business continuity
# User Research and Market Analysis
## User Research
Research Methods used : Desk research, User interview and User survey
### Key Insights
- Desk research : Enterprises are consolidating spend on a few large agent platforms (AWS Bedrock AgentCore, Microsoft Copilot Studio, Salesforce, Google, ServiceNow), not scattered bots. These platforms act as shared foundations for many agents, with governance, observability, and integration baked in—the exact capabilities an AgentOps solution provides internally.
- User interview : On-call engineers need pre-assembled context, not another alert. They want severity, likely cause, dependency status, and next actions surfaced immediately, and management wants visibility at T0, not after the incident ends.
- FormSG survey: 60% of the respondents said they usually learn about the issue only after other users escalate it, which indicates that detection is often reactive rather than system-driven
## De-risking
We considered both internal and external risk.
Internal Risk
- The internal risk came from our stakeholders that may see this as just another SRE tool, that teams may be hesitant to trust autonomous agents on production workflows, and that the platform could be judged too narrow if it only solves incident response.
- We mitigated this by positioning AgentOps as a general-purpose agent platform rather than a single-purpose incident product, showing that the same runtime can support incident response, deployment validation, and security workflows
- We also reduced adoption risk by keeping human-in-the-loop approval gates, full observability, and transparent workflows at the center of the design, so teams can see every agent action and retain control over high-risk steps.
External Risk
- The main external risk is that larger market leaders can come up with similar platform quickly, especially in a category that is still emerging. We mitigate that by not competing on isolated features; instead, AgentOps is built as a trusted operational layer for regulated environments, where the real barrier to adoption is not “can the product do the task?” but “can it be audited, approved, and safely embedded into government workflows
- our moat is the operating model: real-time traceability, human approval gates, structured incident handoffs, and compliance-ready reporting. These are harder to replicate than a dashboard or agent builder because they require workflow design, accountability capture, and integration with formal processes like escalation, reporting, and review
## Stakeholder Buy-in
Which agencies or departments did you reach out to and did they express interest or commitment?
The team pivoted from incident monitoring and management to building a versatile agent platform that addresses needs across SDLC stages, not just the original problem space.
While we secured CEP interest in the initial solution, we haven't found a business owner for the  agent platform solution.
# Solutioning
## Problem-Solution Fit
How does your product specifically address the pain points identified?
Engineering teams often detect issues too late because their operational work is fragmented across manual checks, on-call reactions, deploy reviews, and security scans. AgentOps closes that gap by turning those work to autonomous agents that continuously watch for signals, assemble context, and act on behalf of the team across incident response, deployment validation, security triage, and other operational tasks.
The result is earlier detection, less dependency on who happens to be watching, and a more consistent way to catch and resolve problems before they reach users.
## Functionality
What are your key user flows/features?
- 1. Deploy agent squads from template or build from scratch
  - Users can quickly launch pre-built agent squads for common workflows or create custom agents from scratch to match specific team needs. The platform supports a visual builder with prompts, tools, connectors, policies, so teams can tailor agents for incident response, deployment validation, security triage, or other operational tasks. This makes it easy to go from idea to working agent without heavy engineering overhead.
- 2. Mission control screen
  - The mission control screen gives teams a real-time view of what every agent is doing across the workspace. It shows live agent activity, service status, the incident timeline, and the approval queue in one place, so operators get both transparency and reassurance without switching between tools. This also makes it easy to see how many items are actively waiting for human action, which helps teams prioritize quickly.
- 3. Action detail screen
  - The action detail screen lets users zoom into a specific issue or agent step to see exactly what was detected, what the agent concluded, and what action it wants to take. From there, the platform can either execute the remediation automatically for low-risk actions or pause for approval when the action is high impact or destructive. This gives teams a clear balance of speed and control, with human oversight built into the critical steps
‘
## User Experience
How did you make the experience seamless/intuitive for the end user?
- We made the experience seamless by turning complex SDLC work into a guided, real-time flow rather than asking users to stitch together tools manually. Users can start from a template or build from scratch, see live YAML and step-by-step setup, and then watch agents run with streaming reasoning so there is no black box feeling.
- The interface also keeps the most important decisions in one place: mission control shows live agent activity, health, and the approval queue, while the detail view focuses only on the specific action or issue that needs attention. That reduces context switching and helps users move from detection to decision quickly, with clear approval gates for high-risk actions.
## User Validation
What feedback did users give about the product? What worked well and what required improvement?
Worked well:
- Users like the versatility of the agent platform to create agent based on their specific needs.
Require improvement:
- The initial design has too much information shown in a single page which competing for users' attention, users are confused on which information require attention and which information are just for information.
- The flow of the onboarding process not intuitive.
# Impact & Next Steps
## Success Metrics
What is your "North Star" metric?
- Demonstrate that autonomous AI agents can handle multiple lifecycle workflows - observe, reason, and act - with minimal human intervention, in real time, with full observability and meaningful human oversight.
- For the flagship SRE use case specifically:
  - MTTR (Mean Time To Resolution) reduction from xx minutes down to sub-5 minutes
  - Incident autonomy rate: Percentage of incidents handled end-to-end by agents with only approval gates
## Expected Impact
- For Engineers
  - Faster incident response: Reduce Mean Time To Resolution (MTTR) from 30-60+ minutes to under 5 minutes
  - Less toil, more building: Reduce operational toil freeing up senior engineers for actual engineering work
  - Knowledge that stays: Operational expertise gets codified in the system instead of leaving when experienced engineers leave
- For GovTech
  - Scale without headcount: Handle growing operational load with the same team size
  - Cost efficiency: Reclaim cost currently spent on repetitive toil
  - Risk reduction: Catch bad deploys and critical security vulnerabilities before they reach users
