---
title: "Queue Masters - Queue Me"
description: "Real-time, predictive queue insights that keep voters informed, reduce wait times, and empower polling teams to manage crowds efficiently"
sidebarTitle: "Queue Masters"
icon: "users"
---

# Queue Masters - Queue Me

| Field | Value |
| --- | --- |
| Requested team | Queue Masters |
| Judging group | Final Judging Group 3 |
| Scheduled time | 2:46pm |
| Team number | 68 |
| Category | Social |
| Booth | 8E-09 |
| Project page | [https://build.tech.gov.sg/projects/2026/68](https://build.tech.gov.sg/projects/2026/68) |
| Team members | Adrian Wong; Lydia Li; Patrick Lim; Xiu Xiu Tan; Yanchao Du |

## Summary

Real-time, predictive queue insights that keep voters informed, reduce wait times, and empower polling teams to manage crowds efficiently

## Full Write-Up

# Problem Statement
## Users
2.7m voters and 50k Election Officials
## Use Case
Voters need near real-time, accurate updates on queue lengths and wait times at their polling station. Queue monitoring should be automated in a cost-effective way, reducing reliance on manual reporting by Election Officers.
## Pain Point
The current queue management process suffers from limited visibility and delayed information flow, resulting in reactive operations and suboptimal voter experience.
Key challenges include:
Limited real-time insight into queue conditions
- Queue status is primarily observed manually, reported with delays, and difficult to consolidate or analyze across multiple stations.
Information asymmetry
- Voters cannot access advance insights into expected waiting times.
- Operations teams lack predictive tools and comparative views across locations, reducing their ability to anticipate congestion.
Reactive management approach
- Interventions are typically triggered only after congestion becomes apparent on-site, limiting proactive decision-making and efficiency improvements.
## Consequence
Degraded user experience at scale
- Voters encounter long queues and uncertainty, causing frustration and a negative perception of the process.
Increased operational inefficiency
- Polling staff are overextended managing peak crowds.
- Central teams are forced into reactive, last-minute firefighting rather than strategic oversight.
System-level risk
- Repeated poor queue experiences can erode public confidence in the efficiency and reliability of a critical national process.
# User Research and Market Analysis
## User Research
To validate the need for an improved queue management solution, we analyzed GE2025 operational data.
Research Methods:
Operational Data Analysis
- Examined EO data entry logs, specifically the requirement for EOs to key in queue updates every 5 minutes. Metrics studied included late occurrences and average lag per hour.
Key Insights from Real Users:
  Significant delays in real-time queue updates
    - Across peak hours (12:00–20:00), EOs frequently exceeded the 5-minute update interval, with average lags around 14 minutes and some instances exceeding 85 minutes.
    - Late occurrences were widespread, indicating that manual reporting is difficult to sustain consistently during busy periods.
  High operational load during peak periods
    - Data shows higher late occurrences and max lag during 15:00–20:00, suggesting that EOs struggle to keep up when queues are busiest.
    Conclusion:
The combination of data-driven evidence and frontline observations validates that the current manual system creates lag, friction, and information asymmetry—demonstrating a clear need for a real-time, predictive queue management solution.
## De-risking
1. Adoption Risk
  Risk: Users may not trust or act on new queue information.
    Mitigation:
      - Position the solution as decision support, not a directive.
      - Ensure outputs are simple, interpretable, and aligned with existing workflows.
2. Operational Risk
  Risk: Introducing new tools on polling day could disrupt operations.
  Mitigation:
    - Make the solution additive, complementing current processes.
    - Focus on backend analytics and insights, avoiding changes to frontline procedures.
1. Data Availability Risk
  Risk: Queue data may be incomplete, delayed, or noisy.
  Mitigation:
    - Design for graceful degradation—partial insights remain actionable.
    - Emphasize trends and comparative signals rather than absolute precision
## Stakeholder Buy-in
The ELD business owners, election officials.
# Solutioning
## Problem-Solution Fit
Our product removes the need for officers to constantly observe and manually update queue status by using camera capture of the queue area + AI people counting to generate continuous queue estimates (counts and trends), so officers can focus on on‑site operations while queue visibility remains timely.
## Functionality
1. AI Queue Counting (Officer Burden Reduction)
- Camera captures queue situation in a predefined queue zone (e.g., entry/holding line area).
- AI counts people in the queue zone and outputs:
  - Estimated queue count (near-real-time)
  - Queue trend (increasing / stable / decreasing)
1. Ops/Command Dashboard (Operational Visibility)
      Consolidated view across polling stations with:
- Current estimated queue counts
- Trends for early detection of congestion
hotspots
3. Responsible AI & Privacy Controls (Built-in Feature Set)
- Zone-based counting only; no identity tracking (no facial recognition, no biometric identification).
- Store only aggregated outputs (counts/trends), not identifiable footage.
## User Experience
Designed for “humans under pressure”: keep interaction minimal so officers can update/operate quickly with low cognitive load.
## User Validation
POC findings indicate automated counting is promising but environment-dependent—supporting the need for calibration and zone design
# Impact & Next Steps
## Success Metrics
Timeliness of Queue Information
- Objective: Ensure near-real-time visibility of queue build-up to citizens.
- Reduce average lag between actual queue build-up and system visibility from ~14 minutes → ≤5 minutes.
## Expected Impact
What outcomes do you expect this to be able to deliver in the short/medium/long term if your product is launched to users?
### Short Term (Pilot / Initial Deployment)
Objective: Improve voter experience and transparency at the station.
- Reduced uncertainty
  Voters receive near-real-time queue updates, so they know what to expect.
- Shorter perceived wait times
  Earlier detection of queue build-up helps staff respond faster, making waits feel smoother.
- Enhanced confidence
  Citizens see a transparent and well-managed process, boosting trust in polling operations.
### Medium Term (Scaled Deployment)
Objective: Provide a more predictable and smoother voting experience.
- Proactive crowd management benefits voters
  Reduced extreme queue peaks mean less congestion during busy hours.
- Better flow and service
  Fewer bottlenecks lead to smoother movement through polling stations.
- Consistency across locations
  Standardised queue updates reduce variability, giving voters a reliable experience no matter the station.
### Long Term (Sustained Use & Optimisation)
Objective: Institutionalise a citizen-first, efficient voting experience.
- Reliable, data-driven experience
  Historical queue data enables planning for optimal staffing and station design, minimizing long waits in future elections.
- Increased public confidence
  Transparent, automated monitoring ensures citizens trust the process and feel informed.
