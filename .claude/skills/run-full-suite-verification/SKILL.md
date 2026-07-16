---
name: run-full-suite-verification
description: 프론트엔드 타입 체크와 백엔드 테스트를 순차적으로 실행하여 전체 시스템의 무결성을 검증합니다.
---

1. `cd ~/Desktop/week2/frontend && npx tsc --noEmit 2>&1 | tail -30; rm -f tsconfig.tsbuildinfo`를 실행합니다.
2. `cd ~/Desktop/week2 && web-server/.venv/Scripts/python -m pytest web-server/tests -v 2>&1 | tail -20`를 실행합니다.
3. 위 두 명령어가 모두 성공적으로 완료되었는지 확인합니다.