# Research agent

A single-agent literature investigation pilot with a mobile voice review handoff
(GGS 662, Week 6). Research topic: **[[set in research_brief.md]]**.

## How the handoff works

1. **Local agent:** a coding agent (Claude Code, Codex, etc.) opened in this
   repository reads `AGENTS.md` and `research_brief.md`, then runs
   `prompts/investigate.md`. One agent does the searching, source inspection,
   synthesis, and reporting. It runs interactively, with no unattended API runner.
2. **GitHub:** you review the outputs, then commit and push. Phone assistants read
   the pushed version, not your local folder.
3. **Phone voice review:** connect this repository to ChatGPT (or Claude) and ask:

   > Use the GitHub connection to read reports/latest.md in Jrog378/research-agent.
   > State its run ID, date, and verification phrase, then brief me on it.

   Then question the evidence by voice.
4. **Back to the agent:** summarize the decisions from the voice discussion, correct
   the summary, and save it as `decisions/<run-id>-human-review.md`. The next local
   run reads it. Voice conversations never update this repository automatically.

## Structure

- `AGENTS.md`: scientific research rules for the agent.
- `CLAUDE.md`: tells Claude Code to follow `AGENTS.md`.
- `research_brief.md`: objective, questions, scope, budget, and stopping rules.
- `prompts/investigate.md`: the reusable investigation prompt.
- `runs/<run-id>/`: preserved activity log, evidence register, gap assessment, and briefing.
- `reports/latest.md`: self-contained copy of the latest briefing for phone review.
- `decisions/`: human-reviewed decision summaries between runs.
