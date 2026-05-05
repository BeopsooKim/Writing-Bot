# Writing Bot

**Version:** v1.0.0  
**Created by:** Beopsoo Kim, Department of Electrical and Computer Engineering, Inha University  
**License:** Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)

> **Important notice:** This project is intended for non-commercial research, education, and laboratory training. It is not offered for commercial products, paid services, proprietary internal tooling, or monetized redistribution without separate written permission.

## Overview

Writing Bot is a Codex Skill suite for writing, revision, citation integrity, reviewer response planning, career documents, professional communication, and presentation/poster communication.

Writing Bot is not a ghostwriting service. It is a tutor and editor that helps users think, structure, revise, and communicate more clearly.

## Installation

If you are in a repository root that contains the `Writing-Bot` directory, run:

```bash
mkdir -p .agents/skills
cp -R Writing-Bot/.agents/skills/* .agents/skills/
```

If you are already inside the `Writing-Bot` directory and want to install into the parent repository root, run:

```bash
mkdir -p ../.agents/skills
cp -R .agents/skills/* ../.agents/skills/
```

For personal global installation, run:

```bash
mkdir -p "$HOME/.agents/skills"
cp -R .agents/skills/* "$HOME/.agents/skills/"
```

## Master invocation

```text
$writing-bot
```

## Included Skills

- `writing-bot`: Master router for the Writing Bot suite. It classifies a writing task, detects the stage, and recommends the correct specialized writing skill.
- `writing-triage-router`: Classifies ambiguous writing requests and routes the user to the correct Writing Bot skill.
- `academic-writing-tutor`: Supports academic writing, including paper sections, theses, abstracts, introductions, methods, results, and discussion logic.
- `career-application-writing-coach`: Supports CV, resume, cover letter, SOP, research statement, teaching statement, and interview-answer preparation without ghostwriting.
- `professional-civic-communication-editor`: Supports practical communication such as emails, requests, apologies, notices, meeting messages, and community-facing writing.
- `presentation-poster-communication-designer`: Transforms research or written material into slide, poster, storyboard, visual abstract, and talk-track structures.
- `revision-diagnostics-editor`: Diagnoses a provided draft at the level of claim, evidence, analysis, logic, clarity, tone, and structure.
- `citation-integrity-reviewer`: Checks citation ethics, paraphrasing risk, patchwriting, missing attribution, source reliability, and self-plagiarism risk.
- `reviewer-response-planner`: Helps convert reviewer, editor, advisor, or supervisor feedback into a calm point-by-point response and revision plan.

## Recommended usage

Start with the master router unless you already know the exact workflow. Give the bot the task, audience, current material, constraints, and language context.

## GitHub publication

This repository is prepared for public GitHub release under the repository name `Writing-Bot`. See `GITHUB_PUBLISH.md` for the recommended `gh` workflow.

---

# Writing Bot

**버전:** v1.0.0  
**작성자:** 김법수, 인하대학교 전기컴퓨터공학과  
**라이선스:** 크리에이티브 커먼즈 저작자표시-비영리-동일조건변경허락 4.0 국제 라이선스(CC BY-NC-SA 4.0)

> **중요 고지:** 이 프로젝트는 비상업적 연구, 교육, 연구실 훈련을 위한 자료입니다. 별도의 서면 허가 없이 상업 제품, 유료 서비스, 독점적 내부 도구, 수익화된 재배포에 사용할 수 없습니다.

## 개요

Writing Bot은 글쓰기, 퇴고, 인용 무결성, 리뷰어 대응 계획, 커리어 문서, 전문 커뮤니케이션, 발표/포스터 커뮤니케이션을 위한 Codex Skill Suite입니다.

Writing Bot은 대필 서비스가 아닙니다. 사용자가 스스로 사고하고, 구조화하고, 수정하고, 더 명확하게 소통하도록 돕는 튜터이자 편집 도구입니다.

## 설치

`Writing-Bot` 디렉터리를 포함하는 레포지토리 루트에 있다면 다음을 실행하십시오.

```bash
mkdir -p .agents/skills
cp -R Writing-Bot/.agents/skills/* .agents/skills/
```

이미 `Writing-Bot` 디렉터리 안에 있고 부모 디렉터리의 레포지토리 루트에 설치하려면 다음을 실행하십시오.

```bash
mkdir -p ../.agents/skills
cp -R .agents/skills/* ../.agents/skills/
```

개인 전역 환경에 설치하려면 다음을 실행하십시오.

```bash
mkdir -p "$HOME/.agents/skills"
cp -R .agents/skills/* "$HOME/.agents/skills/"
```

## 대표 호출명

```text
$writing-bot
```

## 포함된 Skill

- `writing-bot`: Writing Bot 전체의 대표 라우터입니다. 글쓰기 작업을 분류하고 현재 단계를 진단한 뒤 적절한 전문 Skill을 추천합니다.
- `writing-triage-router`: 모호한 글쓰기 요청을 분류하고 적절한 Writing Bot 하위 Skill로 연결합니다.
- `academic-writing-tutor`: 논문 섹션, 학위논문, 초록, 서론, 방법론, 결과, 논의 구조 등 학술 글쓰기를 지원합니다.
- `career-application-writing-coach`: CV, resume, cover letter, SOP, research statement, teaching statement, 면접 답변 준비를 대필 없이 지원합니다.
- `professional-civic-communication-editor`: 이메일, 요청문, 사과문, 공지, 회의 메시지, 지역사회 대상 글쓰기 등 실무 커뮤니케이션을 지원합니다.
- `presentation-poster-communication-designer`: 연구 내용이나 글을 슬라이드, 포스터, 스토리보드, graphical abstract, 발표 대본 구조로 변환합니다.
- `revision-diagnostics-editor`: 사용자가 제공한 초안을 주장, 근거, 분석, 논리, 명확성, 어조, 구조 관점에서 진단합니다.
- `citation-integrity-reviewer`: 인용 윤리, paraphrasing 위험, patchwriting, 출처 누락, 출처 신뢰성, 자기표절 위험을 점검합니다.
- `reviewer-response-planner`: 리뷰어, 에디터, 지도교수, 상사의 피드백을 차분한 point-by-point 답변과 수정 계획으로 바꿉니다.

## 권장 사용법

정확한 워크플로우를 이미 알고 있지 않다면 대표 라우터부터 시작하십시오. 작업, 독자, 현재 자료, 제약 조건, 언어 맥락을 함께 제공하는 것이 좋습니다.

## GitHub 공개

이 저장소는 `Writing-Bot`이라는 repository 이름으로 public GitHub 공개가 가능하도록 준비되어 있습니다. 권장 `gh` 절차는 `GITHUB_PUBLISH.md`를 참고하십시오.

