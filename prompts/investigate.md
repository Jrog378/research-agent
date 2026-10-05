# Single-agent investigation prompt

Read AGENTS.md and research_brief.md. Conduct one bounded literature investigation using available web search, source-reading, and local file tools.

Start by inspecting reports/latest.md and previous runs. Choose searches based on unresolved questions and the evidence encountered. Inspect original papers and official dataset documentation. Revise searches when findings challenge the initial framing. Do not simply generate a plausible literature review from memory.

Create a unique run directory under runs/ and write:

1. activity_log.md: actual queries, inspected URLs, access outcomes, concise explanations of search changes, and stopping reason.
2. literature_evidence.md: paper IDs and verified metadata; geography, question, data, methods, findings, validation, limitations, and supporting source locations. Mark unknown fields explicitly.
3. gap_assessment.md: candidate gaps, supporting and competing evidence, search limitations, feasible datasets, and what would invalidate each proposed contribution.
4. briefing.md: an approximately five-minute spoken briefing, followed by detailed evidence and questions requiring human judgment. Use paper IDs and avoid reading long URLs in the spoken portion.

Copy the self-contained briefing to reports/latest.md. Include run ID, date, references, and links to the preserved artifacts. State what was verified and what remains proposed. Do not assert scientific novelty without human review. Report the actions performed and stop within the brief's limits.
