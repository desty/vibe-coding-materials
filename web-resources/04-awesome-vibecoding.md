# Awesome Vibe Coding - 바이브코딩 종합 리소스 가이드

> Source: https://github.com/roboco-io/awesome-vibecoding
> 한국어/일본어 지원 | 주간 자동 업데이트

---

## 바이브코딩이란?

2025년 2월 Andrej Karpathy가 제안한 AI 네이티브 소프트웨어 개발 패러다임.
자연어로 의도를 설명하면 AI가 코드를 생성하는 방식.

### 핵심 특징
- **Natural language first** — 구현 방법이 아닌 원하는 것을 설명
- **Intent-driven specs** — 상세 문서 대신 느슨한 설명
- **Test-based validation** — 사람은 판단, AI는 생성

## 패러다임 비교

| 접근법 | 사람의 역할 | 적합한 경우 |
|--------|-----------|------------|
| 전통 코딩 | 모든 코드 직접 작성/읽기 | 완전한 통제, 프로덕션 시스템 |
| AI 보조 코딩 | 코드 리뷰 및 개선 | 감독 하에 빠른 개발 |
| 바이브 코딩 | 의도로 가이드, 결과 테스트 | 빠른 프로토타이핑, MVP |

## 필수 도구

### IDE & 에디터 어시스턴트
- GitHub Copilot, Cursor, Windsurf (Cascade AI), Claude Code
- 오픈소스: Continue, Cline

### Agentic 코딩 환경
- Devin, OpenHands, Goose — 최소 개입으로 E2E 개발

### MCP (Model Context Protocol) 서버
- Git, DB, 보안 스캔, 브라우저 자동화, 클라우드 인프라 연동

### 클라우드 & 브라우저 플랫폼
- v0, Bolt.new, Lovable, Firebase Studio — 자연어로 앱 생성

## Best Practices

### ✅ DO
- 종합적인 컨텍스트와 아키텍처 세부사항을 사전에 제공
- 계획 → 생성 → 테스트 → 리팩토링 단계로 분리
- 생성된 코드와 함께 또는 먼저 테스트 작성
- 격리된 샌드박스에서 AI 생성 코드 실행
- 비판적 평가로 모든 출력 리뷰
- 아티팩트 문서 유지 (PRD, NOTES, CHANGELOG)

### ❌ DON'T
- 단순해 보이는 코드 리뷰 건너뛰기
- 프롬프트에 시크릿이나 자격증명 포함
- 보호 없이 독점 코드를 공개 모델에 제공
- 검증 없이 AI 출력 수용
- 복잡한 아키텍처 결정을 AI에만 의존

## 추천 워크플로우

### 기능 개발
Vibe Brief → PRD 검증 → Vertical slice 계획 → 단계별 구현

### 리팩토링
패턴 분석 → 안전 전략 → 순차적 개선

### 버그 해결
분류 → 최소 테스트 케이스 → 수정 → 검증

### 테스트 생성
핵심 동작 식별 → 리스크 우선순위 → 테스트 생성
