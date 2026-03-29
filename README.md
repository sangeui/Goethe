# Goethe: Antigravity Agentic OS Boilerplate
(English / 한국어)

> *"Knowing is not enough; we must apply. Willing is not enough; we must do."* 
> *"아는 것만으로는 부족하다, 적용해야 한다. 의지만으로는 부족하다, 실행해야 한다."* 
> — Johann Wolfgang von Goethe (요한 볼프강 폰 괴테)

**Goethe** is a 100% controlled Agentic OS boilerplate for Google Antigravity. It blocks hallucinated AI coding by enforcing strict ideation evaluation, proactive history logging, and version control loops into a single, automated sandbox framework.

**Goethe** (괴테)는 Google Antigravity 에이전트를 위한 100% 통제형 보일러플레이트( Agentic OS 템플릿 )입니다. AI 비서가 지시 없이 무지성으로 코딩하는 것을 원천 차단하고, 가장 엄격한 형태의 기획안 검증, 의사결정 로깅, 버전 관리 자동화를 강제(Lock-up)하는 시스템 뼈대입니다.

> ⚠️ **Language Notice: Built for Korean** / 언어 주의사항
> The internal rules, workflows, and prompts (such as `003-git-convention.md`, `/commit-work`, etc.) are heavily optimized and hardcoded for the **Korean** language. If you intend to use this framework with an English-first agent, you must manually translate the `.agents/rules` and `.agents/workflows` markdown files into English. 
> 
> 본 저장소 내부의 모든 에이전트 페르소나, 워크플로 스크립트, 그리고 003번(Git 100% 한국어) 룰 등은 **한국어로 강하게 결합**되어 있습니다. 다른 언어(예: 영어) 기반의 에이전트로 운용하시려면 `.agents/` 폴더 내 마크다운 룰 파일들의 명령어(Instruction)를 해당 언어로 번역하셔야 정상 작동합니다.

---

## 🛠️ Core Features (핵심 아키텍처)

### 1. 💡 Ideation Hub ( `ideas/` ) 
A controlled sandbox forcing the AI to roleplay as a Product Manager and CTO before any code is generated. (무지성 코딩을 막고 참모진 롤플레잉을 수행하는 통제 샌드박스입니다.)
- **`ideas/AGENTS.md`**: Forcing PM and CTO personas. (PM/CTO 강제 스위칭 라우팅 룰)
- **`ideas/frameworks/`**: PM (JTBD) & CTO (NFR) validation checklists. (기획/기술 타당성 팩트 폭행 검증 문서)
- **`ideas/proposals/`**: Permanent archive for validated ideas. (검증 통과 기획안 영구 보존 아카이브)

### 2. 🤖 Agent Rules ( `.agents/rules/` )
Strict guidelines defining the agent's obligations and user's persona. (사용자의 페르소나와 에이전트 의무 규칙 모음)
- **`000-user-profile.md`**: Implements the rigorous "System Thinker" persona. ("시스템 띵커" 페르소나 기본 탑재)
- **`003-git-convention.md`**: Enforces strict Conventional Commits in Korean. (전면 한국어 지향, 7대 커밋 타입 강제)
- **`004-proactive-commit.md`**: The AI proactively suggests committing their work without being asked. (작업 완료 시 선제적 커밋 대행 자동화 트리거)

### 3. ⚙️ Agent Workflows ( `.agents/workflows/` )
Scripted macro buttons enabling mechanical CI/CD from the AI. (에이전트를 매크로처럼 부리는 스크립트)
- **`/review-idea`**: 1-click meeting evaluating user ideas against PM/CTO frameworks. (아이디어를 참모진 프레임워크로 리뷰하는 기획 회의)
- **`/commit-work`**: End-to-end automated committing: `git status` $\rightarrow$ formatting $\rightarrow$ Agent signature $\rightarrow$ Silent Amend lock. (상태 파악부터 찌꺼기 없는 무한루프 방지 어멘드 락까지 메인 CI 구동)
- **`/log-work`, `/log-decision`**: One-way documentation workflows. (일방향 문서화 및 지식 자산 구축)

### 4. 🧹 Template Cleansing ( `.gitignore` )
Precisely configured to exclude trailing daily logs or old instance knowledge when starting a new project. Only `_TEMPLATE.md` skeletons are preserved in the generic repository. (순백의 템플릿 환경 유지를 위해 파편화된 스냅샷 파일들을 전부 배제합니다.)

---

## 🚀 Getting Started (시작하기)

1. Fork or use this repository as a **Template Repository**. (이 저장소를 Template으로 복제하십시오.)
2. Open a new project directory and spin up the Antigravity agent. (새 프로젝트를 열고 에이전트와 대화합니다.)
3. Go to the `ideas/` folder and pitch a feature. The AI will immediately aggressively validate it. ( `ideas/` 폴더에서 아이디어를 던지면 매우 혹독한 리뷰가 쏟아집니다. )
4. Once tasks are complete, simply permit the agent when it asks: **"Shall I commit this for you?"** (작업 결과 도출 후 에이전트가 예쁘게 커밋해주겠다고 권유하면 그저 "네" 라고 대답하시면 됩니다.)

---
*Created by [sangeui]. Powered by Google Antigravity.*
