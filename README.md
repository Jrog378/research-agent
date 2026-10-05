# Inland-waterway research agent

A pilot for evidence-based literature investigation and mobile voice review.

## First: test the handoff

Connect this repository to ChatGPT through its GitHub connection. Ask:

> Read reports/latest.md in edwardoughton/research_agent using GitHub. State the run identifier and verification phrase, then summarize the report.

Continue that conversation in Voice on your phone. Ask what has actually been verified and what is only proposed. Direct GitHub retrieval in Voice depends on your account; retrieve in text first if necessary. No file uploads are required for this route.

## Run the research agent locally

Open this repository in your coding agent. Use the prompt in `prompts/investigate.md`. The current pilot uses the agent's existing browsing and file tools; it does not call a model API or run unattended. One agent performs searches, source inspection, synthesis, and reporting.

Read `research_brief.md` and `AGENTS.md` first. Preserve each run under `runs/<unique-run-id>/`. Publish a self-contained briefing at `reports/latest.md`. Commit and push reports when the investigation is complete. ChatGPT reads the pushed version, not local changes.

The GitHub connection is a reading handoff. Spoken decisions do not automatically update this repository. Review a decision summary from the phone conversation and supply it to the local agent for the next run.

## Structure

- `research_brief.md`: objective, scope, and constraints.
- `prompts/investigate.md`: reusable single-agent instruction.
- `runs/`: preserved activity logs, literature evidence, and briefings.
- `reports/latest.md`: latest report for mobile discussion.

Scheduled/API-backed execution and a teaching notebook can follow after the phone test succeeds.
