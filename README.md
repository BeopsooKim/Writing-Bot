# Writing Bot

## English

**Version:** v1.0.2  
**Created by:** Beopsoo Kim (`김법수`), Department of Electrical and Computer Engineering, Inha University  
**License:** Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (`CC BY-NC-SA 4.0`)  
**License note:** The binding legal terms follow the official CC license text. Any Korean wording in this repository is explanatory, not a separate legal instrument.

### Important Notice

This project is intended for non-commercial research, education, and laboratory training. It is not offered for commercial products, paid services, proprietary internal tooling, or monetized redistribution without separate written permission.

### Overview

Writing Bot is a Codex skill suite for writing, revision, citation integrity, reviewer-response planning, career documents, professional communication, and presentation or poster communication.

Writing Bot is not a ghostwriting service. It is a structured tutor and editor that helps users think, organize, revise, and communicate more clearly while preserving user authorship and responsibility.

### Repository Structure

- `.agents/skills/writing-bot`: umbrella router for the suite
- `.agents/skills/writing-triage-router`: lightweight routing helper
- `.agents/skills/*`: specialized writing workflows
- `README.md`, `Manual.md`, `EVALS.md`: suite-level documentation and smoke-test references

### Installation

#### Install into Codex global skills

Copy the skill directories under `.agents/skills/` into `~/.codex/skills/`.

```bash
mkdir -p "$HOME/.codex/skills"
cp -R .agents/skills/* "$HOME/.codex/skills/"
```

#### Install into a repo-local agents layout

```bash
mkdir -p .agents/skills
cp -R Writing-Bot/.agents/skills/* .agents/skills/
```

### Master Invocation

```text
$writing-bot
```

### Included Skills

- `writing-bot`: master router for the Writing Bot suite
- `writing-triage-router`: routing helper for ambiguous requests
- `academic-writing-tutor`: academic writing and paper-structure coaching
- `career-application-writing-coach`: CV, SOP, cover-letter, and career-narrative coaching
- `professional-civic-communication-editor`: practical communication editing
- `presentation-poster-communication-designer`: slides, posters, storyboard, and talk-track design
- `revision-diagnostics-editor`: logic, evidence, clarity, tone, and structure diagnosis on existing text
- `citation-integrity-reviewer`: citation ethics, paraphrase risk, attribution, and source integrity
- `reviewer-response-planner`: point-by-point response planning for reviewers, advisors, or editors

### Recommended Usage

Start with the master router unless you already know the exact workflow. Provide the task, audience, current material, constraints, and language context.

### What's New in v1.0.2

- Sharpened core specialist skills with stronger low-RAG operating logic embedded directly in `SKILL.md`.
- Added explicit `verified / manuscript-only / unverifiable` handling and compact Korean evidence-line rules to `citation-integrity-reviewer`.
- Added stable manuscript-anchor logic to `revision-diagnostics-editor` and `reviewer-response-planner` so outputs point to local edit sites instead of vague section names.
- Added stronger bounded-claim export rules and safer title phrasing to `reviewer-response-planner` and `presentation-poster-communication-designer`.
- Corrected the Korean author name in public documentation and package metadata.
- Rewrote public-facing documentation so English and Korean are separated instead of mixed inline.

### Release History

- `v1.0.2`: low-RAG sharpening, claim-bounding improvements, author-name correction, and bilingual public-doc cleanup
- `v1.0.1`: frontmatter cleanup, mojibake cleanup, and broken ZIP artifact removal
- `v1.0.0`: first public release

## 한국어

**버전:** v1.0.2  
**제작자:** Beopsoo Kim (`김법수`), 인하대학교 전기컴퓨터공학과  
**라이선스:** Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (`CC BY-NC-SA 4.0`)  
**라이선스 안내:** 법적 효력은 CC 공식 라이선스 원문에 따릅니다. 이 저장소의 한국어 문구는 설명용이며 별도의 법적 문서가 아닙니다.

### 중요 안내

이 프로젝트는 비상업적 연구, 교육, 연구실 훈련 목적에 한해 제공됩니다. 별도 서면 허가 없이 상용 제품, 유료 서비스, 사내 독점 도구, 수익화된 재배포에 사용할 수 없습니다.

### 개요

Writing Bot은 글쓰기, 수정, 인용 무결성 검토, reviewer-response planning, 커리어 문서 작성 보조, 실무 커뮤니케이션, 발표 및 포스터 커뮤니케이션을 위한 Codex skill suite입니다.

Writing Bot은 대필 서비스가 아닙니다. 사용자 저자성과 책임을 보존한 채, 더 명확하게 사고하고 구조화하고 수정하고 전달하도록 돕는 구조화된 tutor이자 editor입니다.

### 저장소 구조

- `.agents/skills/writing-bot`: suite용 상위 router
- `.agents/skills/writing-triage-router`: 경량 routing helper
- `.agents/skills/*`: 개별 전문 writing workflow
- `README.md`, `Manual.md`, `EVALS.md`: suite 수준 문서와 스모크 테스트 참고 자료

### 설치

#### Codex 전역 skills에 설치

`.agents/skills/` 아래 skill 디렉터리를 `~/.codex/skills/`로 복사합니다.

```bash
mkdir -p "$HOME/.codex/skills"
cp -R .agents/skills/* "$HOME/.codex/skills/"
```

#### 저장소 로컬 `.agents` 레이아웃에 설치

```bash
mkdir -p .agents/skills
cp -R Writing-Bot/.agents/skills/* .agents/skills/
```

### 마스터 호출

```text
$writing-bot
```

### 포함된 Skills

- `writing-bot`: Writing Bot suite의 상위 master router
- `writing-triage-router`: 애매한 요청을 적절한 skill로 보내는 routing helper
- `academic-writing-tutor`: 학술 글쓰기와 논문 구조 코칭
- `career-application-writing-coach`: CV, SOP, cover letter, career narrative 코칭
- `professional-civic-communication-editor`: 실무 커뮤니케이션 편집
- `presentation-poster-communication-designer`: 슬라이드, 포스터, 스토리보드, 발표 메시지 설계
- `revision-diagnostics-editor`: 기존 텍스트의 논리, 근거, 명확성, 어조, 구조 진단
- `citation-integrity-reviewer`: 인용 윤리, 패러프레이즈 위험, attribution, source integrity 검토
- `reviewer-response-planner`: reviewer, advisor, editor 대응용 point-by-point revision planning

### 권장 사용 방식

정확한 workflow를 이미 알고 있지 않다면 master router부터 시작하는 것이 맞습니다. 작업 목표, 독자, 현재 자료, 제약 조건, 언어 맥락을 함께 제공하십시오.

### v1.0.2 업데이트 내역

- 핵심 specialist skill의 low-RAG 동작 규칙을 외부 참조 파일이 아니라 각 `SKILL.md` 내부에 직접 강화했습니다.
- `citation-integrity-reviewer`에 `verified / manuscript-only / unverifiable` 판정과 한국어 compact evidence-line 규칙을 추가했습니다.
- `revision-diagnostics-editor`와 `reviewer-response-planner`에 stable manuscript-anchor 로직을 넣어, 막연한 section 이름 대신 실제 edit site를 가리키도록 강화했습니다.
- `reviewer-response-planner`와 `presentation-poster-communication-designer`에 bounded-claim export 규칙과 더 안전한 제목 문구 규칙을 추가했습니다.
- 공개 문서와 package metadata에 표기된 한국어 작성자명을 `김법수`로 바로잡았습니다.
- 공개 문서를 인라인 혼합형이 아니라 영문/국문 분리 구조로 다시 정리했습니다.

### 릴리스 기록

- `v1.0.2`: low-RAG 고도화, claim-bounding 강화, 작성자명 정정, 공개 문서 이중언어 정리
- `v1.0.1`: frontmatter 정리, mojibake 정리, 손상된 ZIP 산출물 제거
- `v1.0.0`: 첫 공개 릴리스
