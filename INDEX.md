# FLOW PM KIT — INDEX

이 파일은 저장소의 진입점이다. 사람과 AI 모두 먼저 이 파일을 읽고 필요한 규칙/스킬로 이동한다.

## 목적
아이디어 또는 기존 기획을 아래 흐름으로 빠르게 구체화한다.

아이디어
→ Product Document
→ Mobile Screen Spec
→ Web Extension
→ Clickable Prototype
→ Senior Review
→ QA
→ Next Validation

## 핵심 원칙
- Mobile First: 390×844 기준, 360×800 / 430×932 검증
- Web은 모바일 정보구조를 유지하며 확장
- Toss-inspired: 단순함, 명확한 계층, 넉넉한 여백, 빠른 행동
- 화면당 Primary CTA 1개를 기본값으로 사용
- 사실 / 가정 / 확인 필요를 분리
- 프로토타입은 mock/local 우선
- 사용자 승인 전 실배포, 실메일, 실게시, 결제, 삭제 금지
- GitHub가 Source of Truth이며 Vercel 배포는 기본 사용하지 않음

## 기본 규칙
- `AGENTS.md`: 전체 운영 원칙과 Git 규칙
- `README.md`: 저장소 개요와 사용법

## 디자인
- `docs/design/MOBILE_INDEX.md`: 모바일 화면 기준
- `docs/design/WEB_INDEX.md`: 웹 확장 기준
- `docs/design/TOSS_STYLE.md`: UI/UX 스타일 원칙

## OpenCode Skills
- `product-doc`: PRD, 제안서, 요구사항서, 정책서, 보고서
- `mobile-screen-spec`: 모바일 화면설계
- `web-extension`: 웹 확장 설계
- `prototype`: 클릭 가능한 프로토타입
- `senior-review`: 사수형 리뷰
- `qa`: 모바일/웹 QA

## OpenCode Commands
- `/flow`: 전체 PM 파이프라인 실행
- `/prd`: PRD 작성
- `/proposal`: 제안서 작성
- `/requirements`: 요구사항서 작성
- `/policy`: 정책서 작성
- `/report`: 보고서 작성
- `/screen`: 화면설계
- `/prototype`: 클릭형 프로토타입
- `/review`: 사수 리뷰
- `/qa`: QA

## AI가 이 저장소를 사용할 때
1. `AGENTS.md`와 이 `INDEX.md`를 먼저 읽는다.
2. 요청에 필요한 최소 스킬만 사용한다.
3. UI가 포함되면 모바일을 먼저 설계한다.
4. 사용자가 전체 플로우를 요청하면 `/flow`와 동일한 순서로 진행한다.
5. 결과물은 문서 → 화면 → 프로토타입 → 검증의 연결성을 유지한다.
