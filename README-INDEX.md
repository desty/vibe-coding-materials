# 바이브코딩 & Claude Code 교육 자료 모음

> PM 팀 1~2시간 교육용 | 2026년 3월 기준 최신 자료
> 온라인에서 인기 있는 자료들을 수집/정리

---

## 폴더 구조

```
vibe-coding-materials/
├── README-INDEX.md          ← 지금 보고 있는 파일 (총 인덱스)
├── github-repos/            ← GitHub 클론 8개 (전체 소스 포함)
│   ├── claude-howto/              ← Claude Code 종합 가이드 (10개 챕터)
│   ├── claude-code-pm-course/     ← PM 특화 Claude Code 코스
│   ├── claude-code-best-practice/ ← Best Practice 23.7k Stars ⭐
│   ├── everything-claude-code/    ← 50k+ Stars, 해커톤 우승작 ⭐
│   ├── awesome-claude-code/       ← 150+ 큐레이션 리소스
│   ├── awesome-vibecoding/        ← 바이브코딩 종합 리소스
│   ├── awesome-claude-skills/     ← 100+ 실용 스킬 모음
│   └── easy-vibe/                 ← 체계적 바이브코딩 튜토리얼
└── web-resources/           ← 인기 웹 자료 마크다운 변환 (한글 요약)
    ├── 01-claude-code-best-practice-23k-stars.md
    ├── 02-everything-claude-code-50k-stars.md
    ├── 03-awesome-claude-code-5.8k-stars.md
    ├── 04-awesome-vibecoding.md
    ├── 05-awesome-claude-skills-composio.md
    ├── 06-easy-vibe-datawhale-4.6k-stars.md
    └── 07-claude-code-official-docs.md
```

---

## GitHub Repos (Clone 완료)

### 1. claude-howto (luongnv89)
- **URL**: https://github.com/luongnv89/claude-howto
- **내용**: Claude Code 기능별 체계적 학습 가이드
- **구성**: 10개 챕터 (Slash Commands → Memory → Skills → Subagents → MCP → Hooks → Plugins → Checkpoints → Advanced → CLI)
- **특징**: Learning Roadmap, Quick Reference, 슬라이드 포함
- **교육 활용**: 기초~중급, 단계별 실습에 최적

### 2. claude-code-pm-course (carlvellotti)
- **URL**: https://github.com/carlvellotti/claude-code-pm-course
- **내용**: PM을 위한 Claude Code 코스 (★ PM 팀 교육에 직접 활용 가능)
- **구성**:
  - Lesson 1: Fundamentals (첫 작업, 에이전트, 서브에이전트, 네비게이션)
  - Lesson 2: Advanced PM Work (PRD 작성, 프로덕트 전략)
  - Lesson 3: Nano Banana (이미지 생성, PM 유스케이스)
- **특징**: 실습 자료 (유저 인터뷰, 서포트 티켓, 미팅 노트 등) 포함

---

## 웹 자료 (마크다운 변환)

### 01. Claude Code Best Practice (23.7k Stars) ⭐ 필독
- 10 Core Concepts, 12 Hot Features, 86+ Tips
- 8가지 인기 워크플로우 비교표 포함
- **교육 활용**: 팁 & 트릭 위주 속성 교육에 좋음

### 02. Everything Claude Code (50k+ Stars) ⭐ 필독
- Anthropic 해커톤 우승작
- 28 에이전트, 60+ 스킬, 30+ 커맨드
- **교육 활용**: 실전 프로젝트에 바로 적용 가능한 설정/플러그인

### 03. Awesome Claude Code (5.8k Stars)
- 150+ 큐레이션 리소스 모음
- Skills, Hooks, Workflows, Plugins 카테고리별 정리
- **교육 활용**: 참고 링크 모음으로 공유하기 좋음

### 04. Awesome Vibe Coding
- 바이브코딩 개념 소개 + 도구 비교
- Best Practices (Do's & Don'ts) 정리
- **교육 활용**: 바이브코딩 개념 소개 첫 슬라이드용

### 05. Awesome Claude Skills (Composio)
- 33+ 카테고리, 100+ 실용 스킬
- 78+ SaaS 앱 자동화 연동 목록
- **교육 활용**: "이런 것도 가능합니다" 데모 시 참고

### 06. Easy-Vibe (DataWhale, 4.6k Stars)
- 체계적 바이브코딩 튜토리얼
- Stage 0~3 학습 경로, 80+ 인터랙티브 주제
- **교육 활용**: 초보자가 따라할 수 있는 단계별 과정

### 07. Claude Code 공식 문서
- Anthropic 공식 최신 문서 요약
- 설치, 기능, CLI, MCP, Agent Teams, 스케줄링 등
- **교육 활용**: 공식 레퍼런스로 활용

---

## 추가 참고 리소스 (Clone하지 않았지만 유용한 것들)

| 이름 | Stars | URL | 특징 |
|------|-------|-----|------|
| vibe-vibe (DataWhale) | 4.2k | https://github.com/datawhalechina/vibe-vibe | Zero-to-Full-Stack, 16 챕터 |
| ai-guide (Yupi) | - | https://github.com/liyupi/ai-guide | 무료 바이브코딩 코스, ai.codefather.cn |
| Ruflo | - | https://github.com/ruvnet/ruflo | 멀티에이전트 오케스트레이션, 100+ 특화 에이전트 |
| vibe-coding-starter | 335 | https://github.com/PageAI-Pro/vibe-coding-starter | TypeScript 스타터 프로젝트 |
| ai-vibe-coding-101 | - | https://github.com/THU-SIGS-AIID/ai-vibe-coding-101 | 칭화대 프로젝트 기반 튜토리얼 |

---

## 교육 커리큘럼 제안 (1~2시간)

### Part 1: 바이브코딩 소개 (20분)
- `04-awesome-vibecoding.md` 기반 개념 설명
- 전통 코딩 vs AI 보조 코딩 vs 바이브코딩 비교
- Do's & Don'ts

### Part 2: Claude Code 실습 (40분)
- `07-claude-code-official-docs.md` 기반 설치/설정
- `github-repos/claude-code-pm-course/` Lesson 1 활용
- 실습: 간단한 프로젝트에서 Claude Code로 기능 구현

### Part 3: PM 실전 활용 (30분)
- `github-repos/claude-code-pm-course/` Lesson 2 (PRD 작성)
- `01-claude-code-best-practice` 팁 & 트릭 공유
- MCP 연동으로 Jira/Slack 등 업무 도구 활용 데모

### Part 4: Q&A + 자료 공유 (10분)
- 이 폴더 전체를 팀에 공유
- 추가 학습 리소스 안내
