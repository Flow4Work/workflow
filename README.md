# FLOW PM KIT

ChatGPT를 메인 PM/PO Copilot으로 두고 **기획 문서 → 모바일 UX → 웹 확장 → 클릭형 프로토타입 → 사수 리뷰 → QA**까지 이어가는 재사용 작업 키트.

## 핵심 구조

```text
사용자
→ ChatGPT = 메인 PM / 기획 / UX / 판단
→ Flow4Work/workflow = 작업 규칙과 기준의 Source of Truth
→ 결과물
→ 필요할 때만 OpenCode = 로컬 코드 적용 / build / lint / runtime 검증
```

## 기본 원칙
- Mobile First
- 기본 모바일 기준 390×844
- 360×800 / 390×844 / 430×932 검증
- Web 1440×900 확장
- Toss-inspired simplicity, not pixel-copying
- 결과 + 주요 판단 이유
- 사실 / 가정 / 확인 필요 분리
- mock/local 프로토타입 우선
- 승인 전 외부 write 금지
- GitHub가 Source of Truth
- Vercel 배포 없음

## ChatGPT에서 가장 빠른 사용

```text
workflow 기준으로 이 아이디어 전체 기획해줘: [내용]
```

UI 중심:

```text
workflow 기준으로 [기능] 모바일 우선 UI/UX + 웹 확장 + 클릭형 프로토타입까지 만들어줘
```

문서만:

```text
workflow 기준으로 [내용] PRD 만들어줘
```

ChatGPT는 작업 전 최신 `INDEX.md`, `AGENTS.md`와 요청에 필요한 규칙을 확인하고 결과물을 직접 만든다.

## 기본 Workflow

아이디어
→ Product Document
→ Mobile Screen Spec
→ Web Extension
→ Clickable Prototype
→ Senior Review
→ QA
→ Next Validation

## 선택 도구: OpenCode
OpenCode는 메인 Copilot이 아니다. 실제 로컬 프로젝트에서 대량 코드 수정, lint, typecheck, build, runtime 검증이 필요할 때 보조 실행기로 사용한다.

저장소의 `.opencode/skills/`와 `.opencode/commands/`는 OpenCode에서도 같은 작업 방식을 재사용할 수 있게 둔 호환 레이어다.

## 기본 디자인 방향
- 모바일을 원본으로 설계한다.
- 한 화면의 주요 목적은 1개로 제한한다.
- Primary CTA는 원칙적으로 화면당 1개.
- 불필요한 카드, KPI 박스, 배너, 탭을 추가하지 않는다.
- Toss 계열의 단순함, 빠른 이해, 명확한 계층, 충분한 여백을 참고한다.
- 특정 서비스 화면을 그대로 복제하지 않는다.
- 웹은 모바일 정보구조를 유지하며 확장한다.

## Source of Truth
- `INDEX.md`: 전체 진입점
- `AGENTS.md`: 프로젝트 규칙
- `.opencode/skills/`: 재사용 작업 스킬 정의
- `.opencode/commands/`: OpenCode 호환 Slash commands
- `docs/design/`: Mobile / Web / UI 원칙
- `docs/templates/OUTPUT_PACKAGE.md`: 기본 산출물 패키지
- `docs/CHAT_USE.md`: ChatGPT 사용법
