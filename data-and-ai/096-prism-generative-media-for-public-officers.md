---
title: "Prism - Generative Media for Public Officers - Prism"
description: "Prism turns your documents into first draft decks, infographics, images, diagrams, and podcasts, grounded in your material and shaped on your terms."
sidebarTitle: "Prism - Generative Media for Public Officers"
icon: "users"
---

# Prism - Generative Media for Public Officers - Prism

| Field | Value |
| --- | --- |
| Requested team | Prism |
| Judging group | Final Judging Group 2 |
| Scheduled time | 2:13pm |
| Team number | 96 |
| Category | Data & AI |
| Booth | 9C-11 |
| Project page | [https://build.tech.gov.sg/projects/2026/96](https://build.tech.gov.sg/projects/2026/96) |
| Product link | [https://labs.aip.gov.sg/prism](https://labs.aip.gov.sg/prism) |
| Team members | Alicia Lam; Rachel Mf Tan; Sone Kyaw Pye; Sumiko Teng |
| Match status | ambiguous-picked - Multiple exact matches: 96:Prism - Generative Media for Public Officers/Prism | 127:csg pentest innovators/prism |

## Summary

Prism turns your documents into first draft decks, infographics, images, diagrams, and podcasts, grounded in your material and shaped on your terms.

## Full Write-Up

# Problem Statement
## Users
Public officers across Singapore Government agencies. The addressable population is roughly 150,000 public servants; the subset who routinely produce creative knowledge work (decks, infographics, briefings, internal comms, podcasts) is a meaningful fraction across roughly 100 agencies. The canonical user is not defined by role. Policy officers, comms staff, ops officers, analysts, and junior staffers all qualify. They are defined by a shared cold-start problem.
[image](https://wjbbfxaztzhszi7i.public.blob.vercel-storage.com/collab-media/cmnwriy70000304jo9d3irxh4/019e2053-bdf1-702b-b6e1-f80594180498-21cdd77cbc1340d3bd34e0fbe7d90936.png)
The evidence base spans both observed behaviour and stated demand. Across Prism and PlatformAI Studio — where some basic generative media showcases live — 480 officers across 70 agencies are already producing images, infographics, diagrams, and podcasts in the past two months alone, through self-discovery in spite of little marketing. Two structured surveys complement that footprint: 78 officers across 39 agencies on slide workflows, and 16 officers on image generation.
Within the slide-survey cohort, 96.2% produce decks for senior leadership and 74.4% spend half a day or more producing one from scratch. The pain is distributed across job functions, classification levels, agency types, and content modalities rather than concentrated in any one role or surface.
## Use Case
Officers are routinely handed content tasks: a deck for the director, an infographic for internal comms, a visual for a slide, a podcast for a campaign. They have material in hand (a 60-page report, a research summary, last year's deck, a brief), an output expected of them, and a working session of an hour or two to produce something credible. The encounter is episodic but recurring; every new content task brings the same problem back.
## Pain Point
The activation energy to produce a first draft is too high. The blank page is the bottleneck. Available tools fail in three distinct ways. Chatbots (ChatGPT, Claude, Gemini) are non-deterministic and freelance over the officer's material; every refinement is another natural-language prompt and another reroll. Notebook-style grounded tools (NotebookLM) anchor outputs in source material but offer few knobs; the output is take-it-or-leave-it, and slide outputs are image-based with no per-element editability. Consumer creative tools (Canva, Gamma, Tome) produce seemingly polished output but are stylistically very telling.
[image](https://wjbbfxaztzhszi7i.public.blob.vercel-storage.com/collab-media/cmnwriy70000304jo9d3irxh4/019e2054-1778-718f-80eb-8e64424fe79a-73be0aeb618441429a16e63397defc1b.png)
The deeper structural problem is that products like these have set a clear expectation of what "good" looks like for content generation. 64.1% of surveyed officers are already using AI tools for deck creation, with consumer products (ChatGPT, NotebookLM, Claude, Gemini, Microsoft Copilot, Gamma) dominating the mix. Officers have a clear, current sense of what AI-assisted content production should look and feel like, and that sense is being shaped outside the government environment. The bar Prism has to clear is therefore not a compliance bar. It is parity with what officers already know is possible.
Chatbots freelance. Notebook tools auto-pilot. Consumer creative tools are stylistically telling. Prism is the only option that is grounded, controllable, and government-native at once.
## Consequence
Junior staffers continue to absorb hours of overnight deck-rebuilding. Senior officers do not get time back. AI adoption inside the government for content production stalls, not because the technology is not there, but because no one has built the in-government surface that meets officers where the consumer references have set the bar. Each agency that wants to do something AI-creative either reinvents the workflow or skips it.
# User Research and Market Analysis
## Behavioural validation precedes Prism
The PlatformAI Studio footprint introduced above is, in itself, the strongest evidence for Prism's market. The context matters. PlatformAI Studio is a recent platform: it launched at the start of 2026 as a showcase surface for capability demonstration, and only began onboarding the broader public-officer base around three months ago. There has been no formal marketing programme or central rollout behind it.
Despite that, 5051 generative-media outputs have already been produced. The new-user curve is steep: 8 new generative-media users in February, 50 in March, 191 in April — month-on-month multipliers of roughly 6× and then 4×. The pattern Prism is purpose-built to support is happening organically, on a product that has not been promoted.
The work being produced spans the full range of government activity. Generative media users come from regulatory, public-service, legal, defence, education, audit, and corporate-function agencies, and the artifacts they produce range from public-facing campaign collateral and policy explainers to internal training materials, briefing decks, and routine reporting. Across all of them the pattern is the same: officers with material in hand and an output expected of them, using PlatformAI Studio's bare-bones surface to clear the cold-start gap. Prism is the productisation that turns this from "possible if you know how" into "the obvious option for the next officer who walks in."
Between the 39 agencies surveyed and the 70 agencies actively generating on PlatformAI Studio, the evidence covers a substantial fraction of the addressable agency population.
The headline finding is that the underlying capabilities are the most-used features on the platform we already operate. Infographic generation is the single most-used capability category (138 unique users, 49 distinct agencies); image generation ranks among the top three. Prism takes those proven-demand capabilities and wraps them in the customisation harness officers have been asking for.
## Stated demand corroborates the behaviour
To pressure-test that the underlying demand is broad and not confined to early adopters, we ran two structured surveys. The first, focused on slide and content production workflows, returned 78 responses across 39 agencies. The second, focused on image generation, returned 16 responses.
94.9% of the slide-survey respondents rated a secure in-government deck-generation tool as 4 or 5 out of 5 useful; 78.2% rated it 5; mean rating 4.73 out of 5. 74.4% spend half a day or more producing a deck from scratch. 96.2% produce decks for senior leadership. 64.1% already use AI tools for content production, with consumer products dominating the mix over in-government alternatives. On the image side, 93.8% have already tried AI image tools for work, and 68.8% said they would be likely or very likely to use a government-approved AI image tool. The most frequently cited frustration with current options, named by 93.8% of image-survey respondents, was "hard to find something that matches what I need", which is exactly the brief Prism's grounded image generation is built to answer.
The qualitative findings from observed user sessions during the hackathon period reinforce the same story. The cold-start pain is consistent across roles. Officers describe being "at the mercy of the chatbot" with consumer AI, and "feeling lucky" with NotebookLM. Both phrases came up unprompted from different testers. Officers want knobs, not chat. The Smart Composer pipeline (outline → plan review → slide review) emerged from observing that one-shot generation, however good, did not give users the control they wanted at the moments they wanted it. Audiences emerged from user requests. The product originally shipped without them; users repeatedly asked for a way to say "this is for senior leadership" or "this is for ground ops." Audiences are now a top-level surface and a load-bearing differentiator. The four source-purpose roles (content, style reference, structure reference, incorporate) came from watching users try to explain to the model what each uploaded source was for. Surfacing the contract as explicit tags resolved the friction.
## First conversion evidence
We ran six structured Prism walkthrough and user interviews during the hackathon, with officers spanning policy, strategy, operations, communications, and legal/compliance roles across several agencies. Four of the six said they would use Prism on a real RSN work task tomorrow. Estimated time savings if Prism were regularly available averaged roughly 5 hours per officer per week, totalling around 30 hours per week across the cohort against a baseline where 74.4% of surveyed officers spend half a day or more producing a single deck.
"Prism would save me the tedious work of preparing and formatting slides and infographics, freeing me up to focus on the accuracy, clarity and cogency of the contents."
— Legal/Compliance officer, MDDI tester
PlatformAI Studio's 70-agency generative media footprint is Prism's addressable market. The hackathon-window job is to demonstrate the conversion mechanism, and the testers are the early evidence that it works.
## De-risking
Prism faces four risks. We have mitigated three, and we are explicit about the fourth.
1. Is the cold-start problem real and broad? Mitigated. Repeated user testing surfaces the same pain across role types and agency types, and the survey breadth across 39 agencies plus the behavioural footprint across 70 agencies on Studio rule out that we are observing a quirk of one role or one agency.
1. Is grounded multimodal generation buildable inside government infrastructure? Mitigated. The working architecture (Smart Composer pipeline, four-role source model, audience injection, per-modality services for image, infographic, diagram, podcast, slides) is shipping and surviving model changes.
1. Could Gemini's native deck generation collapse the moat? Partially mitigated. Prism's moat is positioned as the customisation harness around the generator, not the generator itself. If Gemini's slide generation gets very good, Prism's value migrates upward (knobs, grounding contract, audiences, government context) rather than evaporating.
1. Continuation past the hackathon. This is the open risk. The harness patterns Prism has built are portable back into PlatformAI Studio if Prism does not get incubated as a standalone product, so the engineering investment is preserved either way.
## Stakeholder Buy-in
- Agencies: MOE (scientific diagrams), Judiciary (infographics and podcasts from legal rulings), and a range of general government offices producing internal decks and infographics across multiple agencies. The underlying generation capabilities themselves have been used by officers across more than 80 agencies on PlatformAI Studio. Prism provides a higher-quality and more targeted UX around capabilities that already have demonstrated demand.
- Platform alignment: Prism is a first-party consumer of PlatformAI APIs (image, audio generation, structured text generation, and others). The relationship is durable; coordination on roadmap is continuous.
# Solutioning
## Problem-Solution Fit
Prism is form-driven (not chat-driven), grounded (via four explicit source-purpose roles), and customisable at every step (Smart Composer plan review, slide review, audience attachment, templates, themes, design references). It targets the cold start, not the finish. Officers walk away from a single working session with a credible first draft they can polish in their tool of choice, or on Prism itself.
[image](https://wjbbfxaztzhszi7i.public.blob.vercel-storage.com/collab-media/cmnwriy70000304jo9d3irxh4/019e2054-8693-749a-931b-474756dce789-a8273ea128b048019bcbe39e3f261d03.png)
The structural defence is closing the gap. Products like Canva, Gamma, ChatGPT, and NotebookLM have set a clear expectation of what good looks like for content generation. When officers cannot find something comparable within government, that gap creates the natural pull toward external tools. Prism's job is to feel just as capable and intuitive as those consumer references, so the in-government option becomes the obvious one. The bar is not compliance; the bar is parity with what officers already know is possible.
## Functionality
Five generation modalities are first-class in the data model: slides, image, infographic, diagram, and podcast.
[image](https://wjbbfxaztzhszi7i.public.blob.vercel-storage.com/collab-media/cmnwriy70000304jo9d3irxh4/019e120f-b511-7161-8faf-6274f55c71be-image%2520%2810%29.png)
The canonical user flow (slide generation, the acquisition driver) is:
1. User creates a project and uploads sources (PDFs, decks, documents, images, transcripts).
1. User tags each source with a purpose role:
  a. content (factual ground truth, or a figure or table to embed verbatim)
  b. style reference (tone and voice to imitate)
  c. structure reference (organisation pattern to follow)
1. User attaches an audience profile (e.g., senior leadership, agency-internal, ground operations) so the generation adapts voice, depth, and terminology.
1. Smart Composer generates an outline from sources, audience, and user intent.
1. Plan review: the user inspects the outline, edits the structure, drops or adds sections, and approves it. This is the load-bearing control surface.
1. Per-slide images are generated.
1. Slide review: the user revises individual slides, regenerates specific ones, or uses inpaint to edit specific elements.
1. User exports to PowerPoint or PDF.
The other modalities (image, infographic, diagram, podcast) follow an analogous pattern: source attachment, generation with explicit knobs, structured review, and export to appropriate file formats, with optional editing or iteration for refinement.
## User Experience
- Form-driven, not chat-driven. Customisation is a knob: a tag, a toggle, a chip. Users configure the model rather than converse with it.
- Grounding contract is visible. The four source-purpose roles surface as tags on each source, so users always know what role each piece of material is playing.
- Anti-expert primacy. Every default biases toward the non-technical officer. Power-user surfaces (JSON prompt editor for image generation, inpaint canvas, source page-range modifiers) are progressively disclosed via modals, never first-class.
- Editorial aesthetic. Light mode only, warm ivory paper-like surfaces, deliberate typography pairing serif display with friendly sans, generous whitespace. The interface signals "workshop," not "admin panel."
- Export to finish. Prism produces drafts. The officer's finishing tool of choice is theirs, not ours. Export paths are first-class.
## User Validation
- The plan review step consistently lands as the "this is the moment I felt in control" feedback. It is the difference between Prism and a chatbot.
- Audiences are engaged with at attachment time and repeatedly cited as the feature that made output feel tailored rather than generic.
- The four source-purpose roles make sense to users without explanation once they have tagged a few sources.
- Podcast generation produces "wait, you can do that?" reactions and broadens user perception of what Prism is for. The 71.4% Studio podcast repeat rate suggests the discovery moment converts to sustained use.
- Among observed testers, the source-extraction stage (mean 4.3 out of 5) and content drafting / outline generation (mean around 4.0) rated highest, validating Smart Composer as the load-bearing surface.
# Impact & Next Steps
## Success Metrics
North star: Generations completed per month, with secondary breakdowns by modality and by agency. This metric captures both adoption breadth (how many users) and engagement depth (how often).
Leading indicators:
- Plan review usage rate (proportion of slide generations where the user inspects or revises the plan before generating slides). Validates that Smart Composer is the moat, not the tax.
- Audience attachment rate (proportion of generations with an audience attached). Validates audiences as a differentiator.
- Word-of-mouth acquisition events (new users acquired through colleague link or share).
Lagging indicators:
- Agencies with sustained usage (≥5 active users producing real outputs in a 30-day window).
- Anchor use case depth: podcasts produced per month for the anchor agency, sustained over time.
## Expected Impact
Short term: Convert the small enthusiastic early-user cohort into a sustained early-adopter base across several agencies. Establish production-usage baselines for the metrics above. Secure committed post-hackathon engineering capacity. Demonstrate the Smart Composer pipeline produces decks users prefer over Gamma and NotebookLM output.
Medium term: Multiple agencies with sustained usage. Anchor podcast agency in steady production use. Senior-leadership-visible demos translate into committed agency adoption. Audiences, templates, and themes prove out as the differentiating muscle versus NotebookLM. Classification posture clarified to a level that lets agencies use Prism for the content they currently produce in external tools.
Long term: Prism becomes the in-government surface officers reach for when they have a content task and a document.
## Next Steps
Prism has received interest from several parties to either further develop as a standalone product, or absorb Prism into existing offerings. We are considering our options at this stage and will likely proceed with a multi-pronged approach to address different user demographics, catering for developers (API and MCP offerings), problem owners (reference designs for prototyping), public officers (opinionated web application).
[file]
