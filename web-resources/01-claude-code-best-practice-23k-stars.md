# Claude Code Best Practice (GitHub 23.7k Stars)

> Source: https://github.com/shanraisshan/claude-code-best-practice
> Updated: 2026-03-27 | 10 Core Concepts, 12 Hot Features, 8 Workflows, 86+ Tips

---

## Core Concepts

Claude Code의 8가지 핵심 기능:

1. **Subagents** - 독립적 컨텍스트에서 작동하는 자율 에이전트. 커스텀 도구, 권한, 지속 ID 보유
2. **Commands** - 기존 컨텍스트에 지식을 주입하는 사용자 호출 프롬프트 템플릿
3. **Skills** - 구성 가능하고 사전 로드 가능한 리소스. 컨텍스트 포크 가능
4. **Workflows** - Commands, Agents, Skills를 조합한 오케스트레이션 패턴
5. **Hooks** - 에이전트 루프 외부에서 특정 이벤트에 실행되는 사용자 정의 핸들러
6. **MCP Servers** - 외부 도구 및 API 연결을 위한 Model Context Protocol
7. **Plugins** - Skills, Subagents, Hooks, MCP 서버를 번들링한 배포 패키지
8. **Settings** - 권한, 모델 설정, 출력 스타일을 포함한 계층적 설정

## Hot Features (2026 최신)

- **Auto Mode** - 수동 권한 프롬프트를 대체하는 백그라운드 안전 분류기
- **Channels** - Telegram, Discord, Webhook에서 활성 세션으로 이벤트 푸시
- **Slack Integration** - 팀 협업 라우팅, Claude Code 세션으로 작업 전달
- **Code Review** - 멀티 에이전트 PR 분석, 버그 및 취약점 식별
- **GitHub Actions** - PR 리뷰 및 이슈 분류 CI/CD 파이프라인 자동화
- **Scheduled Tasks** - 로컬 `/loop` 명령 및 클라우드 `/schedule` 기능
- **Voice Dictation** - 20개 언어 지원 Push-to-Talk 입력
- **Agent Teams** - 공유 코드베이스에서 병렬 에이전트 조율
- **Remote Control** - 디바이스 간 세션 이어가기

## Top Workflow 비교 (Stars 기준)

| Workflow | Stars | 특징 | 핵심 컴포넌트 |
|----------|-------|------|--------------|
| Superpowers | 118k | TDD 우선, Iron Laws | Writing Plans skill |
| Everything Claude Code | 111k | Instinct scoring, AgentShield | Planner agent |
| Spec Kit | 83k | Spec 기반, Constitution | Speckit.plan command |
| gstack | 52k | Role personas, 병렬 스프린트 | Autoplan skill |
| Get Shit Done | 43k | 200K 새 컨텍스트, XML Plans | GSD-planner agent |
| BMAD-METHOD | 43k | Full SDLC, 22+ 플랫폼 | BMAD-create-prd skill |
| OpenSpec | 35k | Delta specs, brownfield | Opsx:propose command |
| Compound Engineering | 11k | Compound Learning | CE-plan skill |

## Tips & Tricks (86개 중 핵심)

### 프롬프팅 전략
- PR 제출 전 테스팅 요구사항으로 Claude에 도전하기
- 초기 수정 후 우아한 재구현 요청하기
- 버그 수정 시 Claude에 자율성 부여하기 (마이크로매니징 금지)

### 계획 및 스펙
- Plan mode로 세션 시작하기
- Claude의 내장 질문 도구로 이해관계자 인터뷰하기
- 여러 테스트 레이어가 있는 단계별 게이트 플랜 구현하기
- 보조 Claude 인스턴스로 시니어 엔지니어급 플랜 리뷰하기

### CLAUDE.md 최적화
- 프로젝트 루트에 CLAUDE.md 배치
- 코딩 표준, 아키텍처 결정, 선호 라이브러리 명시
- 리뷰 체크리스트 포함

### 에이전트 설정
- 서브에이전트별 특화 역할 정의
- 도구 접근 권한 세밀하게 설정
- 병렬 작업 시 에이전트 팀 활용
