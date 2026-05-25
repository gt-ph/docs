---
title: "WiseEats - WiseEats"
description: "Shoppers struggle to make informed nutritional decision because mentally comparing products across inconsistent label formats is slow and unreliable."
sidebarTitle: "WiseEats"
icon: "users"
---

# WiseEats - WiseEats

| Field | Value |
| --- | --- |
| Requested team | Wise Eats |
| Judging group | Final Judging Group 3 |
| Scheduled time | 3:13pm |
| Team number | 7 |
| Category | Healthcare |
| Booth | 8G-11 |
| Project page | [https://build.tech.gov.sg/projects/2026/7](https://build.tech.gov.sg/projects/2026/7) |
| Product link | [https://go.gov.sg/wiseeats](https://go.gov.sg/wiseeats) |
| Team members | Charlene Chua; Chee Hong Wong; Deniece Tan; Jinli Li; Qiaoyun Ye |

## Summary

Shoppers struggle to make informed nutritional decision because mentally comparing products across inconsistent label formats is slow and unreliable.

## Full Write-Up

● Product Name
WiseEats
● Product One-liner (&lt; 150 words)
WiseEats helps grocery shoppers instantly compare nutrition labels and know the healthier choice with no guesswork or math.

● Team Members & Respective Divisions
Chee Hong Wong (GDT-CS), Charlene Chua (GDT-CS), Deniece Tan (GDT-GPO), Jinli Li (GDT-HPB), Qiaoyun Ye (GDT-HPB)
### 1. Problem Statement
● Users: 
Health-conscious consumers of all ages who want to make informed food choices but lack nutritional expertise. This especially includes people managing chronic conditions, fitness enthusiasts, parents shopping for children, and general consumers who want to eat healthier.
● Use Case:
Grocery shoppers compare several similar products to know which one is healthier to purchase. They spend time at the aisle mentally comparing the multiple variables across inconsistent label formats of similar products. The cognitive overload causes them to struggle making a quick decision.
● Pain Points:
- Nutrition labels use inconsistent serving sizes making direct comparison impossible (one bread shows per slice, another per 100g). Shoppers may be comparing the wrong numbers due to misleading/confusing serving sizes that may mask or complicate the nutritional differences
- Technical nutritional terminology without context for what constitutes "high" or "low" amounts
- Information overload with 10+ nutritional values but no clear indication of which are most important, leading to decision paralysis or fatigue leads to defaults rather than informed choices
- Marketing claims like "whole meal," "multigrain," "high fiber" don't correlate clearly with actual nutritional superiority
- Time pressure in stores makes thorough comparison impractical
● Consequences:
Confusing nutrition labels > Poor comparison > Wrong choice > Repeated poor diet > Chronic health risk

Individual (Short-term)
■ Decision paralysis or fatigue leads to defaults rather than informed choices
■ Shoppers may consistently pick products that are higher in sugar, sodium, saturated fats without realising it
■ Shoppers may be comparing the wrong numbers due to misleading/confusing serving sizes that may mask or complicate the nutritional differences

Behavioural (Medium-term)
■ Poor dietary habits from the lack of easily accessible information
■ Shoppers stop reading labels entirely because the effort feels unrewarding

Societal (Long-term)
■ Diet-related chronic diseases
■ Healthcare systems bearing the downstream cost of decisions made in the supermarket aisles
■ Widening health inequality due to information gaps affecting people without nutritional knowledge
### 2. User Research and Market Analysis

● User Research: 
91 online survey respondents, 6 in-depth interviews

Online Survey
Sample: 91 respondents, predominantly aged 40–59 (69%), regular grocery shoppers (70% shop weekly or more frequently). Singapore context, with awareness of local labels (Nutri-grade, Healthier Choice Symbol).

Key Insights:
1. There is a real but underserved behaviour: people want to make healthy choices but lack the tools
Most respondents (63%) read nutrition labels at least sometimes, yet the majority do so only selectively — not systematically. Only 8 people (9%) read labels "always." This gap between intention and action shows that shoppers are motivated but not equipped.
1. Low confidence is pervasive
Only 7 respondents (8%) feel "very confident" identifying the healthier option. Over half (53%) are merely "somewhat confident," and 34% are neutral or not confident. This signals that even engaged shoppers are guessing.
1. Friction points are consistent and addressable
The top barriers to comparing nutrition information, cited across most respondents:
• Small text, hard to read — 57 respondents (63%)
• Don't know what values are "good" or "bad" — 47 respondents (52%)
• Different serving sizes between products — 46 respondents (51%)
• Don't know which nutrients cause health concerns (e.g. trans fat) — 46 respondents (51%)
• Inconsistent nutrient breakdowns across products — 38 respondents (42%)
• Too much information on labels — 35 respondents (38%)
1. Time pressure compounds the problem
Half of respondents (54%) spend less than 3 minutes comparing labels, and 18% make no comparison at all. Shoppers won't read more carefully under time pressure. They need a faster, smarter tool that does the heavy lifting in seconds.
1. Strong and clear demand for the app
67% are interested (37 somewhat + 24 very interested), with only 9% opposed. Neutrals (21%) represent a convertible audience. The demand signal is strong for a core demographic of active, health-conscious shoppers aged 40–59.
In-depth One-to-One Interview
Sample: 6 respondents, predominantly aged 40–59 (83%)

Key Insights:
1. Personalised recommendations over manual comparison Users strongly prefer the app to do the heavy lifting by narrowing down options based on their health profile, goals, and conditions, rather than simply presenting a side-by-side comparison. The real value is reducing decision fatigue and moving users from intent to action quickly.
1. Trust is tied to government backing and transparency Multiple users expressed significantly higher trust in recommendations from a government-linked source. Conversely, influencer endorsements and opaque data practices would undermine trust. Clear communication on how personal data is used is essential.
1. Users have varying literacy around nutrition labels While some users are confident reading labels, others find ingredients lists confusing — particularly additives and "E-numbers" — and struggle with mental math when serving sizes differ. There is a clear need for plain-language explanations, not just raw data.
1. Retention is a genuine challenge Several users noted they would stop using the app once they became familiar with their regular products. To sustain engagement, the app needs to evolve beyond comparison — for example, through meal tracking, whole food nutrition data, or supplement guidance.
1. Fresh produce and supplements are underserved gaps A recurring frustration was the lack of nutritional information for fresh produce, and confusion around supplements. Some users already rely on ChatGPT to fill this gap, suggesting an opportunity to differentiate by covering these categories.
● De-risking: 
- Decision paralysis or fatigue leads to defaults rather than informed choices
- Shoppers may consistently pick products that are higher in sugar, sodium, saturated fats without realising it
- Shoppers may be comparing the wrong numbers due to misleading/confusing serving sizes that may mask or complicate the nutritional differences
● Stakeholder Buy-in: We have reached out to HPB and they have expressed interest.
### 3. Solutioning

● Problem-Solution Fit: 

Standardised comparison through normalisation
Automatically detects and reconciles inconsistent serving sizes across nutrition labels, converting all values to a common baseline (per 100g) before presenting the comparison.
Contextual nutritional guidance
Translates nutritional values into plain-language context, i.e. recommending products based on the health condition or dietary preference.
Cutting Through Marketing Claims
Evaluates products on their actual nutritional data rather than their front-of-pack claims, helping shoppers make decisions based on evidence rather than packaging.
Instant results without guesswork
App instantly presents the nutritional values and recommendations most relevant to common health goals such as sugar, sodium, saturated fat, protein and dietary fibre, significantly reduces the time needed to make an informed choice in-store.
● Functionality:
3-step flow: Scan > Compare > Eat Wiser
● User Experience: 
The experience is built around the simplest possible interaction: snap, compare, decide.
A grocery shopper picks up two similar products, photographs and uploads their nutrition labels, and compares them. There is no manual data entry, and the entire flow takes seconds.
The results screen presents a clean side-by-side comparison at a glance, accompanied by a plain-language write-up explaining not just which product wins, but why. Recommendations are tailored to the user's health goals and dietary preferences, making the guidance personally relevant rather than generic.
The app handles the complexity behind the scenes, reducing cognitive load so shoppers can make a confident, informed choice quickly right there in the aisle.

● User Validation: 
Through usability testing, we have obtained positive responses, with majority emphasises the ease of use.
### 4. Impact & Next Steps

● Success Metric: Frequency of usage
● Expected Impact:
We plan on onboarding approximately 50 shoppers for a pilot across 6 months, with 2 expected outcomes:
Behaviour change at the point of purchase
Majority of active users will make at least one app-assisted healthier product swap within the pilot period, with a target of 60%-70% recommendation acceptance rate. This indicates that users find the guidance trustworthy and actionable.

Habit formation and repeat usage
A monthly active usage rate of 50% or above within the pilot group returning to the app across multiple shopping trips, suggesting the comparison flow is sticky enough to become part of their regular grocery routine.
