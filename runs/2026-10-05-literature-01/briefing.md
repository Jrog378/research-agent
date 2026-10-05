# Inland-waterway research briefing

Run ID: **2026-10-05-literature-01**

Date: October 5, 2026, America/New_York.

Verification phrase: **six sources, one corridor**

Status: completed exploratory literature scan; no empirical analysis or verified novelty claim.

## Spoken briefing

The first finding changes how we should frame the project. Inland-waterway monitoring already exists. A useful project needs to investigate the quality and scientific value of a particular indicator, rather than claim that building a monitor fills an untouched gap.

I searched for inland freight disruption, AIS monitoring and lock-based nowcasting. I retained six research records and inspected official data catalogs. This was a small exploratory search. It is enough to guide a first experiment, but it is not an exhaustive review.

Three papers deserve your attention first. P01 investigates camera-based barge detection. P02 examines estimating barge presence and quantity from vessel tracks. P05 studies disruption and economic consequences. Together they challenge several easy novelty claims: identifying barges, using vessel information and studying disruption are all established research directions. The evidence register explains which records were examined through abstracts and which through selected full-text sections. Detailed performance claims have not been independently reproduced.

P03 and P04 are additional satellite/AIS and tow-size studies. They overlap in authors with the earlier measurement work. We should inspect dataset overlap before treating them as separate confirmations. P06 is the maritime PortWatch comparator. It offers ideas for monitoring, but we cannot simply translate ocean-vessel measurements into inland freight quantities.

The most manageable first prototype would use one corridor and one grain-movement series. It would show observations, a seasonal expectation and departures from that expectation. The scientific question is whether those departures identify documented disruption periods reliably. A chart that looks persuasive is insufficient. We need to count false alerts, check missed events and evaluate results in periods not used to choose the alert threshold.

There are several ways this proposal could fail. Seasonal harvest patterns or changing demand might explain departures. Reporting gaps could resemble interruptions. An event record might refer to a different part of the network. If we tune the system while looking at all historical events, our apparent performance could be optimistic. These risks should determine the first checks.

The data handoff also needs care. USDA provides a convenient catalog, but some movement series originate with USACE. Agreement between those series would not establish independent validity. We need separate evidence about events, and should distinguish a closure or navigation restriction from low water alone.

My recommendation is therefore a data feasibility experiment before a dashboard. Open one workbook, inspect its units and history, and establish whether a usable event reference exists. If those checks succeed, implement a simple retrospective seasonal baseline. If the workbook contains only revised observations, avoid claiming we have measured real-time alert performance.

For teaching, the important agent behavior is visible: evidence changed the proposed direction. The agent began with monitoring as an application, encountered competing work, and narrowed the recommendation to an evaluated question. You retain the decisions about significance, scope and scientific contribution.

## Decisions to discuss by voice

1. Do we prioritize validated disruption detection or estimating freight from vessel observations?
2. Is a grain-specific pilot sufficiently useful for the first teaching example?
3. What would make an alert scientifically credible, and which alternative explanations must it survive?
4. Should the next run inspect P01/P02 in detail or test access to the proposed data?

## Evidence and source links

- P01: Agorku et al., camera detection, preprint 2024 with 2025 journal metadata: https://arxiv.org/abs/2401.03070
- P02: Agorku et al., vessel-track barge estimation, revised preprint 2025: https://arxiv.org/abs/2501.00615
- P03: Agorku et al., satellite/AIS fusion, preprint 2025: https://arxiv.org/abs/2510.11449
- P04: Agorku et al., tow-size regression, preprint 2025: https://arxiv.org/abs/2510.23994
- P05: Chen and Cheng, published disruption study, 2024: https://link.springer.com/article/10.1007/s00168-024-01283-0
- P06: Arslanalp et al., IMF working paper, 2025: https://www.imf.org/-/media/files/publications/wp/2025/english/wpiea2025093-print-pdf.pdf
- D01: Corps Locks report catalog: https://ndc.ops.usace.army.mil/ords/r/lpms/corps-locks/home
- D02: USACE nowcasting overview (search extraction; direct access failed): https://www.iwr.usace.army.mil/About/Technical-Centers/WCSC-Waterborne-Commerce-Statistics-Center/WCSC-Waterborne-Commerce/
- D03: USDA dataset catalog: https://www.ams.usda.gov/services/transportation-analysis/gtr-datasets

## Audit artifacts

Preserved under `runs/2026-10-05-literature-01/`: `activity_log.md`, `literature_evidence.md`, `gap_assessment.md`, and `briefing.md`.

## Voice discussion instructions

Use this report and its evidence register as the source. State the run ID before briefing. Distinguish source-supported findings, agent interpretations and proposed studies. Do not invent methods missing from abstract-level records. Capture proposed human decisions for later review; conversation alone does not update the repository.
