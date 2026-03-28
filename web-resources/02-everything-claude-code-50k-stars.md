# Everything Claude Code (GitHub 50k+ Stars)

> Source: https://github.com/affaan-m/everything-claude-code
> Anthropic Hackathon Winner | 28 Agents, 60+ Skills, 30+ Commands
> Updated: 2026-03 (v1.9.0)

---

## 개요

AI 에이전트 하네스를 위한 종합 성능 최적화 시스템. 프로덕션 레디 설정, 에이전트, 스킬, 자동화 도구를 제공.

## 핵심 구성요소

### Agents (28개)
- **계획 & 아키텍처**: planner, architect
- **코드 품질**: code-reviewer, security-reviewer, refactor-cleaner
- **언어별 리뷰어**: typescript, python, go, java, rust, kotlin, cpp + 각 빌드 에러 리졸버
- **테스트 & 배포**: tdd-guide, e2e-runner, doc-updater
- **운영**: loop-operator, harness-optimizer, chief-of-staff

### Skills (60+)
- **패턴**: Backend, Frontend, API 설계, DB 마이그레이션, Docker
- **언어별**: Django, Laravel, Spring Boot, Go, C++, Python, Rust
- **비즈니스**: 아티클 작성, 콘텐츠 엔진, 시장 조사, 투자자 자료
- **특수**: VideoDb 처리, 보안 스캐닝 (AgentShield)

### Commands (30+)
- `/plan` — 구현 계획
- `/tdd` — 테스트 주도 개발
- `/e2e` — E2E 테스트 생성
- `/code-review` — 품질 평가
- `/build-fix` — 에러 해결
- `/instinct-*` — 학습 패턴 관리

## 설치 방법

```bash
# 플러그인 설치
/plugin marketplace add affaan-m/everything-claude-code
/plugin install everything-claude-code@everything-claude-code

# Rules 수동 설치
git clone https://github.com/affaan-m/everything-claude-code.git
cd everything-claude-code && npm install
./install.sh typescript  # or python, golang, swift, php
```

## 3가지 핵심 가이드

1. **Shorthand Guide** — 설정, 기초, 철학 (먼저 읽기)
2. **Longform Guide** — 토큰 최적화, 메모리 지속, 평가, 병렬화, 서브에이전트 오케스트레이션
3. **Security Guide** — 공격 벡터, 샌드박싱, 살균, CVE, AgentShield 연동

## v1.9.0 주요 업데이트 (2026-03)

- **Selective Install Architecture** — 매니페스트 기반 설치, 타겟 컴포넌트 선택
- **6개 신규 언어 에이전트** — TypeScript, PyTorch, Java, Kotlin
- **12개 신규 스킬** — 딥러닝 패턴, 문서 검색, 모던 JS 툴체인, MCP 서버 패턴
- **SQLite State Store** — 세션 기록 및 스킬 진화 기반
- **12 언어 생태계 Rules** — Java, PHP, Perl, Kotlin/Android, C++, Rust
- 997 내부 테스트 통과

## 고급 기능

### Continuous Learning
세션에서 패턴 자동 추출 → 신뢰도 평가 → 재사용 가능한 스킬로 진화
- `/learn` — 패턴 학습
- `/evolve` — 스킬 진화

### Multi-Agent Orchestration
- `/pm2` — 서비스 라이프사이클 관리
- `/multi-plan` — 태스크 분해
- `/multi-execute` — 조율된 실행

### Security
AgentShield 보안 스캐닝: 102개 규칙, 1282개 테스트
