# Literature and product evidence register

Run: 2026-10-05-literature-01. Exploratory selection; publication status is only what the inspected record establishes. Claims below are paraphrases, not quotations. Unknowns are intentionally retained.

## P01 — Camera-based barge detection

Geoffery Agorku, Sarah Hernandez, Maria Falquez, Subhadipto Poddar, Kwadwo Amankwah-Nkyi. *Traffic Cameras to detect inland waterway barge traffic: An Application of machine learning*. Preprint 2024; repository metadata lists Transportation Research Record 2679(2), 703–720 (2025), DOI 10.1177/03611981241263574.

Source: https://arxiv.org/abs/2401.03070 (abstract and journal-reference fields); PDF retrieved: https://arxiv.org/pdf/2401.03070. Extraction level: abstract; full PDF available but not fully audited.

Mississippi/Ohio camera observations train object detectors; the abstract describes 331 annotated images and weather/location sensitivity checks. It reports YOLOv8 outperforming the tested alternatives. Interpretation: detection of barges is established related work, not an untouched problem. Unresolved: split independence, transfer limits, data reuse rights, and conversion from observations to freight tonnage.

## P02 — AIS-based presence and quantity

Geoffery Agorku, Sarah Hernandez, Maria Falquez, Subhadipto Poddar, Shihao Pang. *Predicting Barge Presence and Quantity on Inland Waterways using Vessel Tracking Data: A Machine Learning Approach*. Submitted December 2024; revised July 2025. Preprint; peer-reviewed publication not established here.

Sources: https://arxiv.org/abs/2501.00615 (abstract/version history); https://arxiv.org/pdf/2501.00615. Extraction level: abstract; PDF retrieved, not comprehensively audited.

Uses camera-derived labels matched to AIS, with staged presence/quantity prediction and movement/vessel features. The abstract reports 164 sampled vessels. Implication: transmitting towboats are not direct observations of all barges or their cargo. Unresolved: vessel-level leakage, held-out geographic/temporal evaluation, AIS licensing, and freight calibration.

## P03 — Satellite/AIS fusion

Geoffery Agorku, Sarah Hernandez, Hayley Hames, Cade Wagner. *Enhancing Maritime Domain Awareness on Inland Waterways: A YOLO-Based Fusion of Satellite and AIS for Vessel Characterization*. October 2025 preprint; peer-reviewed publication not verified.

Source: https://arxiv.org/abs/2510.11449, abstract and submission history. Abstract-only extraction.

Lower Mississippi imagery is combined with AIS. The abstract describes vessel/barge characterization, count estimation, and a geographic transfer assessment. This is competing evidence against treating multimodal inland surveillance as new. Unresolved: acquisition availability, matching uncertainty, evaluation details, and practical temporal refresh rate. Reported capabilities do not establish public real-time deployment.

## P04 — Tow-size regression

Geoffery Agorku, Sarah Hernandez, Hayley Hames, Cade Wagner. *Predicting Barge Tow Size on Inland Waterways Using Vessel Trajectory Derived Features: Proof of Concept*. October 2025 preprint; journal publication not established.

Source: https://arxiv.org/abs/2510.23994, abstract and metadata. Abstract-only extraction; HTML full-text attempt failed.

Lower Mississippi satellite labels are matched with AIS trajectories; models predict barge counts from movement features. Interpretation: tow-size inference already has direct prior work. Unresolved: overlap with P02/P03 datasets, independence of evaluation, generalization, and cargo/loading inference. These related papers should not be counted as independent replications without auditing their data.

## P05 — Disruption and economic consequences

Zhenhua Chen and Junmei Cheng (2024). *Economic consequences of inland waterway disruptions in the Upper Mississippi River region in a changing climate*. The Annals of Regional Science 73, 757–794. Published journal article.

Source: https://link.springer.com/article/10.1007/s00168-024-01283-0. Accessible full-text HTML; inspected sections 5.1, 5.2, 6.2 and limitations. DOI: 10.1007/s00168-024-01283-0.

A seven-lock, 2013–2021 panel combines disruption/environmental observations with barge-rate analysis, spatial econometrics, modal substitution, and economic modeling. Spatial-weight sensitivity is examined. This establishes substantial prior disruption research. Proposed caution: predictive anomaly detection and causal/economic attribution are different objectives; a classroom monitor cannot inherit the article's economic conclusions. Unresolved: reproducing source data, supplementary details, updated lock definitions, and out-of-period evaluation.

## P06 — PortWatch methodological comparator

Serkan Arslanalp, Seung Mo Choi, Parisa Kamali, Robin Koepke, Matthew McKetty, Michele Ruta, Mario Saraiva, Alessandra Sozzi, Jasper Verschuur (2025). *Nowcasting Global Trade from Space*. IMF Working Paper 25/93, May 2025. Working paper, not established as a journal article.

Source: https://www.imf.org/-/media/files/publications/wp/2025/english/wpiea2025093-print-pdf.pdf. Full-text PDF accessible; inspected title, abstract, introduction and limitations, printed pages 2–3.

Port-level AIS-derived indicators underpin maritime-trade nowcasting. Authors distinguish proxies from official statistics and discuss measurement/conversion limitations. Transfer to inland barge freight requires fresh measurement and validation assumptions; vessel activity is not automatically cargo volume. Detailed replication and platform data access remain unchecked.

## D01 — USACE Corps Locks

https://ndc.ops.usace.army.mil/ords/r/lpms/corps-locks/home

Official home page inspected: report catalog describes queue/status, river traffic, monthly tonnage and key-lock reports, annual usage/commodities/unavailability. Download/API behavior and historical completeness not tested. A prototype must add an evaluated question rather than merely reproduce this interface.

## D02 — USACE WCSC nowcasting

https://www.iwr.usace.army.mil/About/Technical-Centers/WCSC-Waterborne-Commerce-Statistics-Center/WCSC-Waterborne-Commerce/

Access limitation: official-page search extraction was readable; two direct opens failed. The extracted Monthly Indicators section describes lock-tonnage-based linear models estimating commodity tonnage, superseded by actual statistics. Treat this as product-discovery evidence needing direct verification before precise replication claims.

## D03 — USDA grain transportation datasets

https://www.ams.usda.gov/services/transportation-analysis/gtr-datasets

Official dataset catalog inspected, particularly Table 9/10 and Figures 12–14. It links grain movements, freight rates, empty barges and New Orleans unloadings. Several movement series originate with USACE, so they are not independent of USACE measurements. Catalog links are verified; workbook schema, units and usable coverage have not been checked. Grain-specific scope cannot represent all commodities.
