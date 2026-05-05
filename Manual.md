# Writing Bot Manual

## English

**Version:** v1.0.2  
**Created by:** Beopsoo Kim (`김법수`), Department of Electrical and Computer Engineering, Inha University  
**License:** Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (`CC BY-NC-SA 4.0`)  
**License note:** The binding legal terms follow the official CC license text. Any Korean wording in this repository is explanatory.

### 1. What This Suite Does

Writing Bot supports writing workflows while preserving user authorship. It separates academic writing, career writing, professional communication, presentation design, revision diagnostics, citation integrity, and reviewer-response planning into focused skills.

### 2. First-Use Workflow

1. Start with the master router.
2. Provide task context, available materials, constraints, and language preference.
3. Let the router select a specialized skill.
4. Use the specialized skill for detailed work.
5. Keep responsibility for final decisions, submissions, and ethical compliance.

### 3. Master Prompt

```text
$writing-bot
Task: [writing task]
Language: [Korean / English / mixed]
Audience: [reader]
Current material: [none / outline / draft / reviewer comments]
Constraint: [deadline / length / format]
Please route me to the right Writing Bot skill.
```

### 4. Skill Selection Guide

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

### 5. Safe-Use Rules

- Do not ask it to write an entire high-stakes academic document from nothing.
- Do not ask it to fabricate sources, statistics, credentials, or experiences.
- Do use it to clarify thesis, evidence, structure, tone, and revision actions.

### 6. Prompt-Quality Rule

Good prompts include the task goal, audience, current material, constraints, and expected output. Bad prompts ask for complete work without context, hide missing evidence, or request unethical shortcuts.

### 7. v1.0.2 Operational Note

This release sharpens low-RAG behavior by pushing more decision logic into `SKILL.md` itself. The specialist skills now rely less on external references and more on explicit conditional rules.

### 8. Maintenance Note

This repository keeps only the suite files that are useful for actual Codex skill operation and smoke testing. Broken ZIP-generated source-module exports were removed during cleanup because they were not load-bearing and were not safely recoverable from the packaged archive.

## 한국어

**버전:** v1.0.2  
**제작자:** Beopsoo Kim (`김법수`), 인하대학교 전기컴퓨터공학과  
**라이선스:** Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (`CC BY-NC-SA 4.0`)  
**라이선스 안내:** 법적 효력은 CC 공식 라이선스 원문에 따르며, 이 저장소의 한국어 문구는 설명용입니다.

### 1. 이 Suite가 하는 일

Writing Bot은 사용자 저자성을 보존하면서 글쓰기 workflow를 지원합니다. 학술 글쓰기, 커리어 문서, 실무 커뮤니케이션, 발표 설계, revision diagnostics, citation integrity, reviewer-response planning을 각각 분리된 전문 skill로 다룹니다.

### 2. 첫 사용 순서

1. master router부터 시작합니다.
2. 작업 맥락, 현재 자료, 제약 조건, 언어 선호를 제공합니다.
3. router가 적절한 전문 skill을 고르게 합니다.
4. 세부 작업은 해당 전문 skill로 진행합니다.
5. 최종 결정, 제출, 윤리 준수 책임은 사용자에게 있습니다.

### 3. 마스터 프롬프트

```text
$writing-bot
Task: [writing task]
Language: [Korean / English / mixed]
Audience: [reader]
Current material: [none / outline / draft / reviewer comments]
Constraint: [deadline / length / format]
Please route me to the right Writing Bot skill.
```

### 4. Skill 선택 가이드

| Skill | 주요 역할 |
|---|---|
| `writing-bot` | Writing Bot suite의 상위 master router |
| `writing-triage-router` | 애매한 writing 요청의 routing |
| `academic-writing-tutor` | 논문, 학위문, 보고서, 초록, 문헌리뷰 |
| `career-application-writing-coach` | CV, resume, cover letter, SOP, career narrative |
| `professional-civic-communication-editor` | 이메일, 요청문, 공지, 사과문, 실무 커뮤니케이션 |
| `presentation-poster-communication-designer` | 슬라이드, 포스터, visual abstract, talk-track 설계 |
| `revision-diagnostics-editor` | 기존 텍스트의 논리, 근거, 명확성, 어조, 구조 진단 |
| `citation-integrity-reviewer` | 인용 윤리, 패러프레이즈 위험, attribution, source reliability |
| `reviewer-response-planner` | point-by-point 답변과 revision planning |

### 5. 안전 사용 규칙

- 아무 근거 없이 고위험 학술 문서를 통째로 작성하라고 시키지 마십시오.
- 출처, 통계, 경력, 경험을 지어내도록 요구하지 마십시오.
- 논지, 근거, 구조, 어조, 수정 액션을 명확히 하는 데 사용하십시오.

### 6. 프롬프트 품질 규칙

좋은 프롬프트는 작업 목표, 독자, 현재 자료, 제약 조건, 기대 산출물을 포함합니다. 나쁜 프롬프트는 맥락 없이 완성본만 요구하거나, 근거 부족을 숨기거나, 비윤리적 지름길을 요구합니다.

### 7. v1.0.2 운영 메모

이번 릴리스는 더 많은 판단 로직을 `SKILL.md` 자체에 밀어 넣어 low-RAG 동작을 강화했습니다. 핵심 specialist skill이 외부 참조 문서보다 명시적 조건부 규칙에 더 의존하도록 바뀌었습니다.

### 8. 유지보수 메모

이 저장소는 실제 Codex skill 동작과 스모크 테스트에 필요한 파일만 유지합니다. ZIP 패키징 과정에서 손상된 source-module 산출물은 핵심 동작에 필요하지 않았고 안전하게 복구할 수 없었기 때문에 정리 과정에서 제거했습니다.
