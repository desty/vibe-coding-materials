# Claude Code 공식 문서 요약

> Source: https://code.claude.com/docs
> Anthropic 공식 | 2026 최신

---

## Claude Code란?

코드베이스를 읽고, 파일을 편집하고, 명령을 실행하고, 개발 도구와 통합하는 에이전틱 코딩 도구.
터미널, IDE, 데스크톱 앱, 브라우저에서 사용 가능.

## 설치 방법

### 터미널 (권장)
```bash
# macOS, Linux, WSL
curl -fsSL https://claude.ai/install.sh | bash

# Windows PowerShell
irm https://claude.ai/install.ps1 | iex

# 프로젝트에서 시작
cd your-project
claude
```

### VS Code / Cursor
Extensions에서 "Claude Code" 검색 후 설치

### 데스크톱 앱
macOS, Windows 다운로드 가능. 비주얼 diff 리뷰, 다중 세션, 스케줄 작업 지원

### 웹
claude.ai/code에서 브라우저로 바로 사용. 로컬 셋업 불필요.

## 핵심 기능

### 1. 자동화
```bash
claude "auth 모듈 테스트 작성하고, 실행하고, 실패 수정해줘"
```
- 테스트 작성, 린트 에러 수정, 머지 충돌 해결, 의존성 업데이트, 릴리스 노트 작성

### 2. 기능 구현 & 버그 수정
자연어로 설명하면 접근법 계획 → 여러 파일 코드 작성 → 검증

### 3. 커밋 & PR
```bash
claude "변경사항을 설명적 메시지로 커밋해줘"
```
GitHub Actions / GitLab CI/CD로 코드 리뷰, 이슈 분류 자동화

### 4. MCP (Model Context Protocol)
Google Drive 문서 읽기, Jira 티켓 업데이트, Slack 데이터 가져오기, 커스텀 도구 연결

### 5. CLAUDE.md로 커스터마이징
프로젝트 루트에 CLAUDE.md 추가 → 코딩 표준, 아키텍처 결정, 선호 라이브러리, 리뷰 체크리스트 설정.
Auto Memory로 빌드 명령, 디버깅 인사이트 자동 저장.

### 6. Skills & Custom Commands
`/review-pr`, `/deploy-staging` 같은 반복 워크플로우 패키징하여 팀 공유

### 7. Hooks
파일 편집 후 자동 포매팅, 커밋 전 린트 실행 등

### 8. Agent Teams
여러 Claude Code 에이전트가 작업 분담, 리드 에이전트가 조율

### 9. CLI 파이프 & 자동화
```bash
# 로그 분석
tail -200 app.log | claude -p "이상 있으면 Slack 보내줘"

# CI에서 번역 자동화
claude -p "새 문자열을 프랑스어로 번역하고 PR 올려줘"

# 보안 리뷰
git diff main --name-only | claude -p "변경 파일 보안 이슈 확인"
```

### 10. 스케줄 작업
- **Cloud** — 컴퓨터 꺼져도 실행. 웹/데스크톱에서 `/schedule`
- **Desktop** — 로컬 머신에서 실행, 로컬 파일 접근
- **`/loop`** — CLI 세션 내 빠른 폴링

### 11. Remote Control
폰에서 이어 작업, Slack에서 `@Claude` 멘션으로 PR 받기, `/teleport`으로 세션 전환

## 사용 환경 비교

| 하고 싶은 것 | 최적 도구 |
|-------------|----------|
| 폰에서 로컬 세션 이어가기 | Remote Control |
| Telegram/Discord 이벤트 세션에 푸시 | Channels |
| 반복 작업 스케줄링 | Cloud/Desktop Scheduled Tasks |
| PR 리뷰 자동화 | GitHub Actions / GitLab CI/CD |
| 모든 PR에 자동 코드 리뷰 | GitHub Code Review |
| Slack 버그 리포트 → PR | Slack 연동 |
| 라이브 웹앱 디버그 | Chrome 연동 |
| 커스텀 에이전트 구축 | Agent SDK |
