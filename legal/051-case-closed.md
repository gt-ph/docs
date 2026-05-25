---
title: "Case Closed - Justifi"
description: "Justifi is a conversational AI assistant that helps self-represented litigants in Small Tribunals prepare clear & legally coherent witness statements"
sidebarTitle: "Case Closed"
icon: "users"
---

# Case Closed - Justifi

| Field | Value |
| --- | --- |
| Requested team | Case Closed |
| Judging group | Final Judging Group 3 |
| Scheduled time | 1:20pm |
| Team number | 51 |
| Category | Legal |
| Booth | 8A-01 |
| Project page | [https://build.tech.gov.sg/projects/2026/51](https://build.tech.gov.sg/projects/2026/51) |
| Product link | [https://app.gvt-build26-case-closed.stg.paas.sandbox.gov.sg/](https://app.gvt-build26-case-closed.stg.paas.sandbox.gov.sg/) |
| Team members | Alexa Charles From.businessedge; Elizabeth Tan Judiciary; Joshua Na; Nurhida Yacob; Pradeep Kaur |

## Summary

Justifi is a conversational AI assistant that helps self-represented litigants in Small Tribunals prepare clear & legally coherent witness statements

## Full Write-Up

# Problem Statement
## Users
Justifi is built for the more than 10,000 self-represented litigants (SRPs) and witnesses who navigate Singapore's small tribunals each year without legal representation.
A secondary user group is about 100 court staff, who currently bear the burden of helping these parties improve their submissions before proceedings can move forward.
## Use Case
Preparing a witness statement is one of the most error-prone steps for self-represented litigants and witnesses. Most submit free-form narratives that are incomplete, disorganized, or hard to follow, leading court staff to spend valuable time clarifying before proceedings can move forward.
Justifi steps in at the moment litigants or witnesses sit down to prepare their statements for trial, replacing the blank page with a conversational assistant that guides them to tell their story clearly and completely - reducing the burden on court staff and improving the quality of statements from the outset.
## Pain Point
1. The core problem lies with self-represented litigants and witnesses who struggle to translate their experience into a clear, structured statement. Guided questions and explanatory notes are available, but many litigants and witnesses find them difficult to follow - either due to limited legal literacy or language barriers.
1. Litigants may simply not know how to write in a legally coherent way. Even those comfortable speaking English may lack the ability to express themselves with the clarity and structure a case requires.
1.  Compounding this, the stress of the court process itself often further undermines their ability to present their case effectively.
## Consequence
The consequences fall on everyone involved:
1. Courts receive poorly structured submissions that require clarification, slowing proceedings and increasing the workload on court staff who spend additional time clarifying and engaging
parties.
1. Litigants risk having their cases misunderstood, their claims weakened, or their submissions rejected - not because their case lacks merit, but because they lack the ability to write and present it well.
# User Research and Market Analysis
## User Research
We interviewed key Judiciary stakeholders – an Assistant Registrar, a Tribunal Magistrate, a District Judge, and front-line officer, to validate the problem.
Their feedback was consistent: witness statement preparation is a significant pain point, and existing guides and explanatory notes are not enough. Approximately 80% of cases present with unclear or unrelated statements, requiring court staff to spend additional time engaging parties before proceedings can move forward.
The downstream impact is clear. Litigants who submit well-prepared statements typically need only one consultation session to move forward. Those with poorly prepared statements require up to three, which is a substantial effort to both the litigant and the court.
## De-risking
Justifi is built on two core assumptions.
1. The first is that the burden of preparing a legal statement is painful enough that Self-represented litigants will adopt a new tool to ease it - given the documented difficulty and the volume of cases, this demand is well-supported.
1. The second is that litigants will trust an AI tool with something as sensitive as their legal statement. Justifi addresses this directly through its design philosophy: the system never adds or embellishes facts. It structures and clarifies what the user has already said, and the user reviews and approves every version before submission. Control always stays with the user.
## Stakeholder Buy-in
Judiciary stakeholders have expressed interest in this solution.
# Solutioning
## Problem-Solution Fit
Justifi meets litigants and witnesses where they are. Rather than asking them to conform to a legal structure with explanatory notes they don't understand, it invites them to tell their story and then does the work of organising that story into a clear, legally coherent statement. It guides without replacing, structures without distorting, and supports without overwhelming.
## Functionality
1. Litigants log in through the existing Case Management System, while witnesses access Justifi via a link shared by litigant. Both are authenticated through SingPass. Upon login, a case-linked context is automatically created, grounding the conversation in the specifics of their matter from the start.
1. Using multimodal AI, Justifi reviews these materials and identifies gaps or additional facts the party (litigant or witness) should address.
1. The party can interact with Justifi via voice or text in any of Singapore's four official languages, removing language as a barrier to participation.
1. As the conversation unfolds, Justifi's agentic engine structures the party's inputs into a formatted statement in line with court guidelines, displayed as a live document alongside the chat.
1. The party retains full editorial control - they can edit the document directly or ask Justifi to make specific changes through the chat.
1. Throughout the process, Justifi can answer questions about legal terms and procedural requirements in plain, accessible language.
1. Once the party is satisfied with their statement, they can submit it to be sent to the Case Management System , no additional steps required.
## User Experience
By allowing the party involved to log in through a single system, and having them to chat with the chatbot in the language that they are comfortable in. The chat engine will also be able to answer queries from parties should they have any doubts on legal terms.
Justifi is designed to feel like a conversation, not a form. A single SingPass login connects the party to their case without friction. Multilingual voice and text input ensures the tool is accessible regardless of language proficiency or digital literacy. The side-by-side chat and document view lets the party watch their statement take shape in real time, turning an intimidating process into one they can feel confident about.
## User Validation
User testing with the prototype is currently being planned. Findings will be incorporated after the testing.
# Impact & Next Steps
## Success Metrics
Justifi will measure its success by two things:
1. Reduction in time court staff spend on clarification and back-and-forth with parties, and
1. Increase in the proportion of statements submitted that meet the required standard without further intervention.
## Expected Impact
In the short term, Justifi aims to meaningfully reduce the per-case burden on court staff, freeing their capacity for higher-value work. For litigants, it delivers reduced risk of misrepresentation, greater confidence in the submission process, and faster case progression. At scale, Justifi has the potential to strengthen access to justice across all the tribunals (Small Claims, Employment Claims, and Community Dispute Resolution). Justifi works to address the pain point in party's submission - ensuring that every party, regardless of background or legal literacy, is able to present their case as clearly and completely as possible.
