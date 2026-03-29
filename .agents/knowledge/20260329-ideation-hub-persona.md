---
title: "Smith Ideation Hub (폴더 기반 페르소나 스위칭 아키텍처)"
date: 2026-03-29
tags: [architecture, persona, ideation]
status: active
---

# Context (맥락)
개발 착수 전 아이디어가 기술적으로 불가능하거나 사업성이 없는 경우를 방지하려면, 무조건 긍정하는 '코더(Coder)' 자아 대신 비판적인 '참모(Executive Board)' 자아가 필요함. Antigravity 1.21.6의 폴더 전용 지침 파일(`AGENTS.md`) 릴리스를 기반으로 이 문제를 해결하고자 함.

# Decision (결정 사항)
사용자가 `Smith/ideas/` 디렉토리 내에서 대화하거나 기획안을 작성할 때, 에이전트가 코딩을 유보하고 **'Product Manager(기획)'와 'CTO(기술)'의 이중 페르소나**로 강제 전환되도록 해당 폴더에 전용 `AGENTS.md`를 심어둠. 

# Constraints & Consequences (제약 조건 및 영향)
* **Positive**: 쓰레기 코드 양산을 방지하고, 초기 기획의 리스크(UX 결함, 기술 비용 등)를 선제적으로 제거함.
* **Constraints**: 이 폴더 안에서 에이전트는 절대 사용자의 아이디어에 맹목적으로 동의(Yes-man)해서는 안 되며, 비판적 팩트 체크와 함께 무조건 '2~3개의 현실적 대안(Trade-off)'을 제시할 의무를 가짐.
