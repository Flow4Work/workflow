# FLOW PM KIT — INDEX

이 파일은 저장소의 진입점이다. **ChatGPT가 메인 PM/PO Copilot**이며, 이 저장소를 최신 작업 기준의 Source of Truth로 사용한다.

## 역할
- ChatGPT: 기획, 판단, UX, 문서, 프로토타입 설계, 리뷰
- GitHub `Flow4Work/workflow`: 작업 규칙과 기준 저장소
- OpenCode: 필요할 때만 로컬 코드 적용/검증을 맡는 선택 실행기

## 기본 흐름
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

## ChatGPT가 읽는 순서
1. `INDEX.md`
2. `AGENTS.md`
3. 요청에 필요한 `.opencode/skills/*/SKILL.md`
4. UI 작업이면 `docs/design/MOBILE_INDEX.md`, `WEB_INDEX.md`, `TOSS_STYLE.md`
5. 결과 패키지는 `docs/templates/OUTPUT_PACKAGE.md`

`.opencode/skills/`는 이름과 위치만 OpenCode 호환 형식을 사용하며, ChatGPT도 동일한 작업 규칙으로 사용한다.

## 작업 스킬
- `product-doc`: PRD, 제안서, 요구사항서, 정책서, 보고서
- `mobile-screen-spec`: 모바일 화면설계
- `web-extension`: 웹 확장 설계
- `prototype`: 클릭 가능한 프로토타입
- `senior-review`: 사수형 리뷰
- `qa`: 모바일/웹 QA

## OpenCode 선택 명령
OpenCode가 필요한 경우에만 사용한다.
- `/flow`: 전체 PM 파이프라인
- `/prd`, `/proposal`, `/requirements`, `/policy`, `/report`
- `/screen`, `/ui`, `/prototype`, `/review`, `/qa`

## ChatGPT 기본 해석
- `workflow 기준으로 기획해줘` → 필요한 규칙을 읽고 ChatGPT가 직접 수행
- UI 포함 → 모바일 먼저, 이후 웹 확장
- 전체 요청 → 문서 → 화면 → 프로토타입 → 리뷰 → QA 순서
- 실제 코드 적용이 크거나 로컬 검증이 필요할 때만 OpenCode 활용
