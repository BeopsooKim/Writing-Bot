# GitHub Publishing Guide

**Repository name:** `Writing-Bot`  
**Visibility:** Public  
**Owner:** `BeopsooKim`  
**Release version:** `v1.0.0`

## English

This folder is ready to be published as a standalone public GitHub repository.

### Fastest workflow

From inside this `Writing-Bot` folder, run:

```bash
./publish_to_github.sh
```

### Manual GitHub CLI workflow

From inside this `Writing-Bot` folder, run:

```bash
git init
git add .
git commit -m "Initial public release v1.0.0"
gh repo create BeopsooKim/Writing-Bot --public --description "Writing Bot: Korean/English Codex Skill suite for writing, revision, citation integrity, reviewer response, career writing, professional communication, and presentation/poster workflows." --source=. --remote=origin --push
git tag v1.0.0
git push origin v1.0.0
```

If GitHub CLI is not authenticated, run:

```bash
gh auth login
```

Choose GitHub.com, HTTPS, and web-browser OAuth authentication.

If you are starting from the combined package root, first enter the suite folder:

```bash
cd Writing-Bot
```

## Korean

이 폴더는 독립적인 public GitHub repository로 바로 공개할 수 있도록 준비되어 있습니다.

### 가장 빠른 절차

이 `Writing-Bot` 폴더 안에서 다음을 실행하십시오.

```bash
./publish_to_github.sh
```

### 수동 GitHub CLI 절차

이 `Writing-Bot` 폴더 안에서 다음을 실행하십시오.

```bash
git init
git add .
git commit -m "Initial public release v1.0.0"
gh repo create BeopsooKim/Writing-Bot --public --description "Writing Bot: Korean/English Codex Skill suite for writing, revision, citation integrity, reviewer response, career writing, professional communication, and presentation/poster workflows." --source=. --remote=origin --push
git tag v1.0.0
git push origin v1.0.0
```

GitHub CLI 인증이 되어 있지 않다면 다음을 실행하십시오.

```bash
gh auth login
```

GitHub.com, HTTPS, web-browser OAuth 인증을 선택하면 됩니다.

통합 패키지 루트에서 시작했다면 먼저 Suite 폴더로 이동하십시오.

```bash
cd Writing-Bot
```
