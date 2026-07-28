# ChatGPT에서 FLOW PM KIT 사용

이 저장소는 ChatGPT가 참고하는 **우리 PM/UX 작업 기준의 Source of Truth**다.

## 가장 간단한 호출

> `workflow 기준으로 이 아이디어 기획해줘: [내용]`

UI까지:

> `workflow 기준으로 모바일 우선 UI/UX + 웹 확장 + 클릭형 프로토타입까지 만들어줘: [내용]`

전체 패키지:

> `workflow 기준으로 처음부터 끝까지 진행해줘: [내용]`

## ChatGPT가 작업할 때
1. 최신 `INDEX.md`와 `AGENTS.md`를 확인한다.
2. 요청에 필요한 스킬만 읽는다.
3. UI가 있으면 Mobile First로 설계한다.
4. 결과물을 ChatGPT가 직접 작성/생성한다.
5. 대량 코드 수정이나 로컬 build/runtime 검증이 필요할 때만 OpenCode를 보조 실행기로 사용한다.

## 기본 해석
- `기획해줘` → 제품 문서
- `PRD` → PRD
- `제안서` → 제안서
- `요구사항서` → 요구사항서
- `정책서` → 정책서
- `보고서` → 보고서
- `화면/UI/UX` → 모바일 UX → 웹 확장
- `프로토타입` → 클릭형 프로토타입
- `검토해줘` → 사수 리뷰
- `QA` → QA
- `처음부터 끝까지` → 전체 파이프라인

## 기본값
- Mobile First
- 390×844 기준
- Toss-inspired simplicity
- Mobile → Web 순서
- 사실 / 가정 / 확인 필요 분리
- 실배포 없이 mock/local 프로토타입 우선
