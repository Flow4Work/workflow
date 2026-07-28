# ChatGPT / 다른 AI에서 FLOW PM KIT 꺼내 쓰기

이 저장소 자체를 Source of Truth로 사용한다.

## 가장 간단한 호출

다음처럼 말하면 된다.

> `Flow4Work/workflow의 FLOW PM KIT 기준으로 이 아이디어 기획해줘: [내용]`

UI까지 필요하면:

> `Flow4Work/workflow 기준으로 모바일 우선 UI/UX + 웹 확장 + 클릭형 프로토타입까지 만들어줘: [내용]`

전체 패키지가 필요하면:

> `Flow4Work/workflow의 전체 FLOW PM 파이프라인으로 진행해줘: [내용]`

## AI가 읽어야 하는 순서
1. `INDEX.md`
2. `AGENTS.md`
3. 필요한 `.opencode/skills/*/SKILL.md`
4. UI 작업이면 `docs/design/MOBILE_INDEX.md`, `WEB_INDEX.md`, `TOSS_STYLE.md`
5. 결과 패키지는 `docs/templates/OUTPUT_PACKAGE.md`

## 기본 해석
- `기획해줘` → product-doc
- `PRD` → `/prd`
- `제안서` → `/proposal`
- `요구사항서` → `/requirements`
- `정책서` → `/policy`
- `보고서` → `/report`
- `화면/UI/UX` → `/ui`
- `화면설계` → `/screen`
- `프로토타입` → `/prototype`
- `검토해줘` → `/review`
- `QA` → `/qa`
- `처음부터 끝까지` → `/flow`

## 중요한 기본값
- Mobile First
- 390×844 기준
- Toss-inspired simplicity
- Mobile → Web 순서
- 사실 / 가정 / 확인 필요 분리
- 실배포 없이 mock/local 프로토타입 우선
