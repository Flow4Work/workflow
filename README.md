# FLOW PM KIT

AI와 함께 **기획 문서 → 모바일 UX → 웹 확장 → 클릭형 프로토타입 → 사수 리뷰 → QA**까지 이어가는 재사용 가능한 PM/PO 작업 키트.

## 핵심
- Mobile First
- 기본 모바일 기준 390×844
- 360×800 / 390×844 / 430×932 검증
- Web 1440×900 확장
- Toss-inspired simplicity, not pixel-copying
- 결과 + 주요 판단 이유
- 사실 / 가정 / 확인 필요 분리
- 승인 전 외부 write 금지
- mock/local 프로토타입 우선
- GitHub가 Source of Truth
- Vercel 배포 없음

## 가장 빠른 사용

OpenCode에서 이 저장소를 clone한 뒤 프로젝트 루트에서 실행한다.

### 전체 파이프라인
```text
/flow 만들고 싶은 아이디어 또는 기존 기획
```

아이디어
→ Product Document
→ Mobile Screen Spec
→ Web Extension
→ Clickable Prototype
→ Senior Review
→ QA
→ Next Validation

### 문서
- `/prd 아이디어`
- `/proposal 제안 내용`
- `/requirements 기능/서비스`
- `/policy 정책 주제`
- `/report 자료/현황`

### UI / Prototype
- `/ui 기능/문서` — 모바일 UX → 웹 확장 → 프로토타입
- `/screen 기능/문서`
- `/prototype 기능/문서`

### 검토
- `/review 산출물`
- `/qa 대상`

## ChatGPT / 다른 AI에서 사용
저장소를 기준으로 다음처럼 요청한다.

```text
Flow4Work/workflow의 FLOW PM KIT 기준으로 이 아이디어 기획해줘: [내용]
```

전체 실행:

```text
Flow4Work/workflow의 전체 FLOW PM 파이프라인으로 진행해줘: [내용]
```

UI 중심:

```text
Flow4Work/workflow 기준으로 모바일 우선 UI/UX + 웹 확장 + 클릭형 프로토타입까지 만들어줘: [내용]
```

자세한 사용법은 `docs/CHAT_USE.md`, 전체 파일 지도는 `INDEX.md` 참고.

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
- `.opencode/skills/`: 재사용 작업 스킬
- `.opencode/commands/`: Slash commands
- `docs/design/`: Mobile / Web / UI 원칙
- `docs/templates/OUTPUT_PACKAGE.md`: 기본 산출물 패키지
