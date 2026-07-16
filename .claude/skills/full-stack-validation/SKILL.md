---
name: full-stack-validation
description: 프론트엔드 타입 체크와 백엔드 테스트를 순차적으로 실행하여 전체 시스템의 무결성을 검증합니다.
---

1. `cd ~/Desktop/week2/frontend && npx tsc --noEmit`을 실행하여 프론트엔드 타입 에러를 확인합니다.
2. 오류 발생 시 `rm -f tsconfig.tsbuildinfo`를 실행합니다.
3. `cd ~/Desktop/week2 && web-server/.venv/Scripts/python -m pytest web-server/tests`를 실행하여 백엔드 테스트를 수행합니다.