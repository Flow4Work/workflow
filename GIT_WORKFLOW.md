# Git Workflow

## 원칙
`main` = 언제 clone해도 사용할 수 있는 안정 버전.

작업 흐름:
1. main 최신화
2. 작업 branch 생성
3. 하나의 논리적 변경만 수행
4. 로컬/OpenCode 검증
5. commit
6. push
7. PR
8. diff + 결과 확인
9. squash merge
10. branch 삭제

Branch:
- `feat/<feature>`
- `fix/<problem>`
- `docs/<topic>`
- `refactor/<area>`

예:
- `feat/mobile-prototype-skill`
- `docs/toss-ux-rules`
- `fix/qa-viewport-rules`

Commit:
- `feat: add mobile-first prototype skill`
- `docs: refine web extension rules`
- `fix: prevent speculative metrics`

## Agent 운영
AI가 수정할 때도 main 직접 변경보다 branch/PR을 우선한다.
PR 본문에 아래를 적는다.

- Why
- What changed
- Files changed
- Verification
- Known limitations

Vercel은 연결하지 않는다.
GitHub Actions도 현재 기본값으로 추가하지 않는다.
