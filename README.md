# Goethe: Antigravity Agentic OS Boilerplate

> *"아는 것만으로는 부족하다, 적용해야 한다. 의지만으로는 부족하다, 실행해야 한다."* 
> — 요한 볼프강 폰 괴테 (Johann Wolfgang von Goethe)

**Goethe**는 Google Antigravity 에이전트를 위한 100% 통제형 보일러플레이트입니다. 
AI 비서가 지시 없이 무지성으로 코딩하는 것을 원천 차단하고, 가장 엄격한 형태의 **기획안 검증, 의사결정 로깅, 100% 한글 버전 관리 자동화**를 물리적으로 강제(Lock-up)하는 시스템 뼈대입니다. 언제든 이 저장소를 포크(Fork)하여 완벽하게 제어되는 AI 코딩 샌드박스로 사용하십시오.

---

## 🛠️ 핵심 아키텍처 (Core Features)

### 1. 💡 Ideation Hub (`ideas/`) 
AI가 무지성 코딩을 시작하지 못하게 막고, 참모진 롤플레잉을 수행하는 통제 샌드박스입니다.
- **`ideas/AGENTS.md`**: 이 폴더 내부에서 대화 시 AI를 'Product Manager'와 'CTO'로 강제 스위칭시키는 라우팅 룰.
- **`ideas/frameworks/`**: PM의 JTBD 프레임워크와 CTO의 NFR(비기능 요구사항) 검증 문서. 로직에 따라 AI는 사용자의 아이디어를 들으면 무조건 이 문서 2개를 먼저 읽어 팩트 폭행을 시작합니다.
- **`ideas/proposals/`**: 검증을 통과한 기획안이 영구 보존되는 아카이브.

### 2. 🤖 Agent Rules (`.agents/rules/`)
사용자의 페르소나와 에이전트의 의무 규칙 모음집입니다.
- **`000-user-profile.md`**: "시스템 띵커(System Thinker)"라는 가장 엄격하고 구조적인 사용자 페르소나 기본 탑재.
- **`003-git-convention.md`**: 전면 100% 한국어 지향, 7대 커밋 타입(feat, fix 등) 강제.
- **`004-proactive-commit.md`**: 유의미한 작업 완료 시, 에이전트가 단독으로 로컬 커밋 대행(`git add/commit`)을 선제적으로 제안하는 자동화 트리거.

### 3. ⚙️ Agent Workflows (`.agents/workflows/`)
버튼처럼 구동하여 에이전트를 매크로처럼 부리는 스크립트입니다.
- **`/review-idea`**: 새로운 아이디어를 참모진 프레임워크로 리뷰하고, 표로 결과물을 반환하는 원클릭 기획 회의.
- **`/commit-work`**: `git status` 파악 $\rightarrow$ 한국어 메시지 생성 $\rightarrow$ 자동 커밋 시그니처(`🤖`) 덧붙임 $\rightarrow$ Silent Amend(무한루프 로깅 방지)까지 완벽히 처리하는 메인 CI 도구.
- **`/log-work`, `/log-decision`**: 일방향 문서화 및 지식 자산 구축 스크립트.

### 4. 🧹 Template Cleansing (`.gitignore`)
저장소를 포크하여 새 프로젝트를 시작할 때, 이전 작업의 흔적이 오염되지 않도록 설계된 정밀 차단망입니다. 특정 날짜가 찍힌 일일 업무일지(`.agents/logs/`)나 지식 자산(ADR)은 원격 깃허브에 영구적으로 올라가지 않으며, 오직 `_TEMPLATE.md` 뼈대 파일들만 안전하게 보존됩니다.

---

## 🚀 시작하기 (Getting Started)

1. 현재 저장소를 GitHub의 **Template Repository**로 지정하거나 Fork 합니다.
2. 새 프로젝트 폴더를 열고 Antigravity 에이전트에게 인사를 건넵니다.
3. `ideas/` 폴더에 들어가서 *"이런 서비스를 기획 중인데 어때?"* 라고 질문해 보세요. 즉시 PM/CTO로 돌변한 에이전트의 혹독한 검증 리포트가 시작됩니다.
4. 작업이 하나씩 끝날 때마다 에이전트가 스스로 **"제가 직접 예쁘게 003번 룰(한국어)로 커밋해 드릴까요?"** 라고 묻습니다. 그저 **"네"** 한마디만 하십시오.

---
*Created by [sangeui]. Powered by Google Antigravity.*
