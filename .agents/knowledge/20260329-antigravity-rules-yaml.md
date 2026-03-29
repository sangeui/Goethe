---
title: "Antigravity 커스텀 룰(Rules) YAML Frontmatter 작성 원칙"
date: 2026-03-29
tags: [architecture, convention, troubleshooting]
status: active
---

# Context (맥락)
커스텀 룰(`.agents/rules/` 하위 마크다운 문서)을 작성했을 때, 오른쪽 사이드바의 `Customizations → Rules` UI 목록에 룰 뱃지가 정상적으로 파싱/노출되지 않는 현상이 발생함. 이는 워크플로(Workflow) 파일과 동일하게 YAML 헤더에 `description`만 작성했기 때문임. 

# Decision (결정 사항)
Antigravity 에이전트의 규칙(패시브 제약 조건)으로 적용될 모든 마크다운 파일은, YAML Frontmatter에 `trigger: always_on` (또는 `trigger: ["path"]` 등 트리거 조건 명시) 속성을 반드시 포함하여 작성되어야 함. 

# Constraints & Consequences (제약 조건 및 영향)
* **Positive**: 오른쪽 사이드바에서 개발자가 룰의 적용 상태를 즉시 모니터링할 수 있으며, 봇 컨텍스트 로딩이 강제됨.
* **Constraints**: 에이전트는 앞으로 새로운 룰 파일(.agents/rules/*.md)을 백그라운드에서 작성/생성할 때, 워크플로 템플릿의 `description:` 대신 **반드시 헤더에 `trigger:`를 포함**시켜야만 함. (이 제약 사항을 무시할 시 UI가 고장 남)
