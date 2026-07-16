---
name: full-stack-validation
description: 프론트엔드 타입 검사와 백엔드 테스트를 순차적으로 실행하여 전체 시스템의 무결성을 확인합니다.
---

1. `cd ~/Desktop/week2/frontend && npx tsc --noEmit`으로 타입 에러를 확인합니다.
2. `rm -f ~/Desktop/week2/frontend/tsconfig.tsbuildinfo`로 빌드 캐시를 정리합니다.
3. `cd ~/Desktop/week2 && web-server/.venv/Scripts/python -m pytest web-server/tests -v`를 실행하여 백엔드 테스트를 통과하는지 확인합니다.