---
title: "ReceiptSG - ReceiptSG"
description: "ReceiptSG is a nationwide digital receipts platform that allows citizens to get their digital receipts with just a tap of their phone"
sidebarTitle: "ReceiptSG"
icon: "users"
---

# ReceiptSG - ReceiptSG

| Field | Value |
| --- | --- |
| Requested team | Receipt SG |
| Judging group | Final Judging Group 1 |
| Scheduled time | 2:13pm |
| Team number | 1 |
| Category | Economy & Finance |
| Booth | 10F-14 |
| Project page | [https://build.tech.gov.sg/projects/2026/1](https://build.tech.gov.sg/projects/2026/1) |
| Team members | Jeremy Jee; Pei Sze Teo; Say Han Foo; Winston Liu |

## Summary

ReceiptSG is a nationwide digital receipts platform that allows citizens to get their digital receipts with just a tap of their phone

## Full Write-Up

# Problem Statement
## Users
500 million retail transactions a year
## Use Case
Whenever any citizen interacts with a retail shop or business, and a receipt is generated
## Pain Point
Paper waste being created without consent, and having to put the burden of tracking expenses on citizens
## Consequence
We increase our carbon footprint without bringing much quality of life benefits to citizens.
# User Research and Market Analysis
## User Research
- Observational research at retail points — how often do citizens discard receipts immediately?
- Interviews with merchants on pain of paper roll costs, printer maintenance, and thermal paper waste
- Survey of citizens on receipt retention habits and expense tracking friction
- Discovery that citizens want to track spending but find manual entry (apps like Seedly) too burdensome
## De-risking
[table block omitted in flat markdown; see narrativeBlocks in JSON]
## Stakeholder Buy-in
- NEA (National Environment Agency) — paper waste reduction aligns with Zero Waste Masterplan
- IMDA — digital economy / cashless infrastructure
- Enterprise Singapore — SME digitalisation push
- Specific merchant chains for pilot (e.g., hawker centre operators, retail chains)
# Solutioning
## Problem-Solution Fit
[table block omitted in flat markdown; see narrativeBlocks in JSON]
## Functionality
Key user flows:
1. Merchant setup (one-time): Sign up → get device token → configure printer app → done
1. Transaction (automatic): POS prints → printer app parses ESC/POS data → uploads to cloud → broadcasts URL via NFC
1. Citizen receipt (tap): Tap phone on terminal → browser opens receipt → auto-claimed if logged in
1. Citizen wallet: View all claimed receipts, search/filter by merchant or category, see spending analytics
1. Admin oversight: Approve business registrations, view platform-wide KPIs, monitor receipt volume
## User Experience
[table block omitted in flat markdown; see narrativeBlocks in JSON]
## User Validation
What worked well:
- "I didn't have to do anything — I just tapped and the receipt was there"
- Merchants appreciated no new hardware requirement
- Spending insights gave citizens a reason to keep using it beyond receipt storage
What required improvement:
- iOS NFC requires a physical tag sticker (platform limitation) — less magical than Android HCE
- First-time users confused about why they should sign up (iterated to show value prop of analytics upfront)
- Business approval flow needed streamlining for faster onboarding
# Impact & Next Steps
## Success Metrics
North Star Metric: Number of receipts claimed per month (represents both merchant adoption and citizen engagement in a single number)
Supporting metrics:
- Merchant activation rate (device tokens created → first receipt issued)
- Citizen retention (% of users who claim 2+ receipts per week)
- Paper saved (receipts issued digitally × avg thermal paper per receipt)
## Expected Impact
[table block omitted in flat markdown; see narrativeBlocks in JSON]
