# Writing Bot Manual

**Version:** v1.0.1  
**Created by:** Beopsoo Kim, Department of Electrical and Computer Engineering, Inha University  
**License:** Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)

## 1. What this suite does

Writing Bot supports writing workflows while preserving user authorship. It separates academic writing, career writing, professional communication, presentation design, revision diagnostics, citation integrity, and reviewer response planning into focused skills.

## 2. First-use workflow

1. Start with the master router.
2. Provide task context, available materials, constraints, and language preference.
3. Let the router select a specialized skill.
4. Use the specialized skill for detailed work.
5. Keep responsibility for final decisions, submissions, and ethical compliance.

## 3. Master prompt

```text
$writing-bot
Task: [writing task]
Language: [Korean / English / mixed]
Audience: [reader]
Current material: [none / outline / draft / reviewer comments]
Constraint: [deadline / length / format]
Please route me to the right Writing Bot skill.
```

## 4. Skill selection guide

| Skill | Primary role |
|---|---|
| `writing-bot` | Master router for the Writing Bot suite. |
| `writing-triage-router` | Routes ambiguous writing requests. |
| `academic-writing-tutor` | Academic papers, theses, reports, abstracts, and literature reviews. |
| `career-application-writing-coach` | CV, resume, cover letter, SOP, and career narrative. |
| `professional-civic-communication-editor` | Email, requests, notices, apologies, and professional communication. |
| `presentation-poster-communication-designer` | Slides, posters, visual abstracts, and talk-track design. |
| `revision-diagnostics-editor` | Logic, evidence, clarity, tone, and structure diagnosis on existing text. |
| `citation-integrity-reviewer` | Citation ethics, paraphrase risk, attribution, and source reliability. |
| `reviewer-response-planner` | Point-by-point response and revision planning. |

## 5. Safe-use rules

- Do not ask it to write an entire high-stakes academic document from nothing.
- Do not ask it to fabricate sources, statistics, credentials, or experiences.
- Do use it to clarify thesis, evidence, structure, tone, and revision actions.

## 6. Prompt-quality rule

Good prompts include the task goal, audience, current material, constraints, and expected output. Bad prompts ask for complete work without context, hide missing evidence, or request unethical shortcuts.

## 7. Maintenance note

This repository keeps only the suite files that are useful for actual Codex skill operation and smoke testing. Broken ZIP-generated source-module exports were removed during cleanup because they were not load-bearing and were not safely recoverable from the packaged archive.
