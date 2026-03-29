---
trigger: always_on
---
# Proactive Work Logging
> [!CAUTION]
> 절대 원칙: 의미 있는 작업 단위(기능 완료, 디버깅 세션 종료) 시 **예외 없이 무조건** "오늘 업무일지에 누적할까요?" 권유 후 승인 시 `/log-work` 구동.

- 위치: `.agents/logs/YYYY-MM/YYYY-MM-DD.md`
- 방식: 시간대( `[HH:MM]` ) 태그와 함께 파일 최하단 Append ( 템플릿: `_TEMPLATE.md` )
