# Optional Writing Skill Routing Guidance

Use this file only if this repository frequently involves writing or communication tasks.

For writing-related requests:
- Prefer the most specific writing skill in `.agents/skills`.
- Do not use multiple writing skills unless the user asks for a multi-stage workflow.
- Preserve the user's authorship in high-stakes academic, career, or evaluated writing.
- Never fabricate citations, data, credentials, experiences, or sources.
- If a writing request is ambiguous, use `writing-triage-router` first.

Recommended routing:
- Academic paper/thesis/report/abstract -> `academic-writing-tutor`
- Resume/CV/cover letter/SOP/interview -> `career-application-writing-coach`
- Email/memo/announcement/request -> `professional-civic-communication-editor`
- Slides/poster/storyboard -> `presentation-poster-communication-designer`
- Pasted draft for critique/rewrite -> `revision-diagnostics-editor`
- Citation/paraphrase/plagiarism/authorship -> `citation-integrity-reviewer`
- Reviewer/professor/supervisor feedback -> `reviewer-response-planner`
