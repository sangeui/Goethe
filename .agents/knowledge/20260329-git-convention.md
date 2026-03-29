---
title: "Git Commit Convention (전면 한국어 및 타입 강제)"
date: 2026-03-29
tags: [git, convention, SOP]
status: active
---

# Context (맥락)
무의미한 텍스트("업데이트", "버그 수정") 사용이나, 영문/국문 혼용으로 인한 Git 로그 가독성 저하를 방어하기 위함. 또한 개발자(인간)와 에이전트(AI)가 완전히 동일한 양식의 커밋을 생성하게 만들어 추적 가능한 히스토리를 유지하기 위함.

# Decision (결정 사항)
1. **타입(Type)**: `feat`, `fix`, `refactor`, `style`, `docs`, `test`, `chore`의 7가지 Conventional Commits 규격을 사용한다.
2. **언어 제한**: 어떠한 경우에도 제목과 본문은 **100% 한국어**로만 작성한다. 
3. **템플릿 연동**: `.gitmessage`를 프로젝트 전역 템플릿으로 할당하여 `git config commit.template`에 의거, 휴먼과 에이전트의 강제 양식으로 고정한다. (`003-git-convention.md` 상주 룰 기반 작동)

# Constraints & Consequences (제약 조건 및 영향)
* **Positive**: 개발 내역이 그대로 마크다운 형식의 깔끔한 한국어 릴리즈 노트(Release Note)로 변모함.
* **Constraints**: 에이전트는 무조건 003번 룰을 지켜서 커밋 메시지를 생성해야 하며, 사용자가 습관적으로 `-m "update"`를 치려 해도 VIM 템플릿에 의해 경각심을 가지게 됨.
