# Writing Bot

**Version:** v1.0.1  
**Created by:** Beopsoo Kim, Department of Electrical and Computer Engineering, Inha University  
**License:** Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)

> **Important notice:** This project is intended for non-commercial research, education, and laboratory training. It is not offered for commercial products, paid services, proprietary internal tooling, or monetized redistribution without separate written permission.

## Overview

Writing Bot is a Codex skill suite for writing, revision, citation integrity, reviewer response planning, career documents, professional communication, and presentation/poster communication.

Writing Bot is not a ghostwriting service. It is a tutor and editor that helps users think, structure, revise, and communicate more clearly.

## Repository structure

- `.agents/skills/writing-bot`: umbrella router for the suite
- `.agents/skills/writing-triage-router`: lightweight routing-only helper
- `.agents/skills/*`: specialized writing workflows
- `README.md`, `Manual.md`, `EVALS.md`: suite-level docs and smoke tests

## Installation

### Install into Codex global skills

Copy the skill directories under `.agents/skills/` into `~/.codex/skills/`.

```bash
mkdir -p "$HOME/.codex/skills"
cp -R .agents/skills/* "$HOME/.codex/skills/"
```

### Install into a repo-local agents layout

If you maintain a repository-local `.agents/skills/` layout, copy the suite there instead.

```bash
mkdir -p .agents/skills
cp -R Writing-Bot/.agents/skills/* .agents/skills/
```

## Master invocation

```text
$writing-bot
```

## Included skills

- `writing-bot`: master router for the Writing Bot suite
- `writing-triage-router`: routing-only helper for ambiguous requests
- `academic-writing-tutor`: academic writing and paper-structure coaching
- `career-application-writing-coach`: CV, SOP, cover-letter, and career-narrative coaching
- `professional-civic-communication-editor`: practical communication editing
- `presentation-poster-communication-designer`: slides, posters, storyboard, and talk-track design
- `revision-diagnostics-editor`: structure, logic, clarity, and evidence diagnosis on existing text
- `citation-integrity-reviewer`: citation ethics, paraphrase risk, attribution, and source integrity
- `reviewer-response-planner`: point-by-point response planning for reviewers, advisors, or editors

## Recommended usage

Start with the master router unless you already know the exact workflow. Provide the task, audience, current material, constraints, and language context.

## Notes on v1.0.1 cleanup

- Removed invalid extra fields from `SKILL.md` frontmatter.
- Cleaned mojibake from operational skill files and suite documentation.
- Removed broken `source-modules/` exports that were not used by the installed skills and were corrupted during ZIP packaging on Windows.
