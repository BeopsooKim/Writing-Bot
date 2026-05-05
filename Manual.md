# Writing Bot Manual

**Version:** v1.0.0  
**Created by:** Beopsoo Kim, Department of Electrical and Computer Engineering, Inha University  
**License:** Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)

> **Important notice:** This project is intended for non-commercial research, education, and laboratory training. It is not offered for commercial products, paid services, proprietary internal tooling, or monetized redistribution without separate written permission.

## 1. What this suite does

Writing Bot supports writing workflows while preserving user authorship. It separates academic writing, career writing, professional communication, presentation design, revision diagnostics, citation integrity, and reviewer response planning into focused Skills.

## 2. First-use workflow

1. Start with the master router.
2. Provide task context, available materials, constraints, and language preference.
3. Let the router select a specialized Skill.
4. Use the specialized Skill for detailed work.
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
| `writing-bot` | Master router for the Writing Bot suite. It classifies a writing task, detects the stage, and recommends the correct specialized writing skill. |
| `writing-triage-router` | Classifies ambiguous writing requests and routes the user to the correct Writing Bot skill. |
| `academic-writing-tutor` | Supports academic writing, including paper sections, theses, abstracts, introductions, methods, results, and discussion logic. |
| `career-application-writing-coach` | Supports CV, resume, cover letter, SOP, research statement, teaching statement, and interview-answer preparation without ghostwriting. |
| `professional-civic-communication-editor` | Supports practical communication such as emails, requests, apologies, notices, meeting messages, and community-facing writing. |
| `presentation-poster-communication-designer` | Transforms research or written material into slide, poster, storyboard, visual abstract, and talk-track structures. |
| `revision-diagnostics-editor` | Diagnoses a provided draft at the level of claim, evidence, analysis, logic, clarity, tone, and structure. |
| `citation-integrity-reviewer` | Checks citation ethics, paraphrasing risk, patchwriting, missing attribution, source reliability, and self-plagiarism risk. |
| `reviewer-response-planner` | Helps convert reviewer, editor, advisor, or supervisor feedback into a calm point-by-point response and revision plan. |

## 5. Safe use rules

- Do not ask it to write an entire academic assignment from nothing.
- Do not ask it to fabricate sources, statistics, credentials, or experiences.
- Do use it to clarify thesis, evidence, structure, tone, and revision actions.

## 6. Prompt quality rule

Good prompts include the task goal, audience, current material, constraints, and what kind of output is expected. Bad prompts ask for complete work without context, hide missing evidence, or request unethical shortcuts.

## 7. Lab maintenance

Collect useful prompts, failure cases, and recurring lab workflows. Add them to `EVALS.md` or a lab examples file. Keep each Skill focused on one workflow.

---

# Writing Bot 사용 설명서

**버전:** v1.0.0  
**작성자:** 김법수, 인하대학교 전기컴퓨터공학과  
**라이선스:** 크리에이티브 커먼즈 저작자표시-비영리-동일조건변경허락 4.0 국제 라이선스(CC BY-NC-SA 4.0)

> **중요 고지:** 이 프로젝트는 비상업적 연구, 교육, 연구실 훈련을 위한 자료입니다. 별도의 서면 허가 없이 상업 제품, 유료 서비스, 독점적 내부 도구, 수익화된 재배포에 사용할 수 없습니다.

## 1. 이 Suite가 하는 일

Writing Bot은 사용자의 저자성을 유지하면서 글쓰기 워크플로우를 지원합니다. 학술 글쓰기, 커리어 글쓰기, 전문 커뮤니케이션, 발표 설계, 퇴고 진단, 인용 무결성, 리뷰어 대응 계획을 전문 Skill로 분리합니다.

## 2. 첫 사용 절차

1. 대표 라우터부터 시작합니다.
2. 작업 맥락, 사용 가능한 자료, 제약 조건, 언어 선호를 제공합니다.
3. 라우터가 전문 Skill을 선택하게 합니다.
4. 전문 Skill로 세부 작업을 진행합니다.
5. 최종 결정, 제출, 윤리 준수 책임은 사용자에게 있음을 유지합니다.

## 3. 대표 프롬프트

```text
$writing-bot
Task: [writing task]
Language: [Korean / English / mixed]
Audience: [reader]
Current material: [none / outline / draft / reviewer comments]
Constraint: [deadline / length / format]
Please route me to the right Writing Bot skill.
```

## 4. Skill 선택 가이드

| Skill | 주요 역할 |
|---|---|
| `writing-bot` | Writing Bot 전체의 대표 라우터입니다. 글쓰기 작업을 분류하고 현재 단계를 진단한 뒤 적절한 전문 Skill을 추천합니다. |
| `writing-triage-router` | 모호한 글쓰기 요청을 분류하고 적절한 Writing Bot 하위 Skill로 연결합니다. |
| `academic-writing-tutor` | 논문 섹션, 학위논문, 초록, 서론, 방법론, 결과, 논의 구조 등 학술 글쓰기를 지원합니다. |
| `career-application-writing-coach` | CV, resume, cover letter, SOP, research statement, teaching statement, 면접 답변 준비를 대필 없이 지원합니다. |
| `professional-civic-communication-editor` | 이메일, 요청문, 사과문, 공지, 회의 메시지, 지역사회 대상 글쓰기 등 실무 커뮤니케이션을 지원합니다. |
| `presentation-poster-communication-designer` | 연구 내용이나 글을 슬라이드, 포스터, 스토리보드, graphical abstract, 발표 대본 구조로 변환합니다. |
| `revision-diagnostics-editor` | 사용자가 제공한 초안을 주장, 근거, 분석, 논리, 명확성, 어조, 구조 관점에서 진단합니다. |
| `citation-integrity-reviewer` | 인용 윤리, paraphrasing 위험, patchwriting, 출처 누락, 출처 신뢰성, 자기표절 위험을 점검합니다. |
| `reviewer-response-planner` | 리뷰어, 에디터, 지도교수, 상사의 피드백을 차분한 point-by-point 답변과 수정 계획으로 바꿉니다. |

## 5. 안전한 사용 규칙

- 빈 상태에서 학술 과제 전체를 작성해 달라고 요청하지 마십시오.
- 출처, 통계, 경력, 경험을 조작해 달라고 요청하지 마십시오.
- 논지, 근거, 구조, 어조, 수정 행동을 명확히 하는 데 사용하십시오.

## 6. 좋은 프롬프트 원칙

좋은 프롬프트는 작업 목표, 독자, 현재 자료, 제약 조건, 기대 출력 형식을 포함합니다. 나쁜 프롬프트는 맥락 없이 완성본을 요구하거나, 근거 부족을 숨기거나, 비윤리적 우회로를 요청합니다.

## 7. 연구실 유지보수

유용한 프롬프트, 실패 사례, 반복되는 연구실 워크플로우를 모으십시오. 이를 `EVALS.md` 또는 연구실 예시 파일에 추가하십시오. 각 Skill은 하나의 워크플로우에 집중하도록 유지해야 합니다.

