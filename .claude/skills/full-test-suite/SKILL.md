---
name: full-test-suite
description: 프론트엔드 타입 검사와 백엔드 테스트를 순차적으로 실행하여 전체 시스템의 무결성을 확인합니다.
---

1. `cd ~/Desktop/week2/frontend && npx tsc --noEmit 2>&1 | tail -30; rm -f tsconfig.tsbuildinfo`를 실행하여 프론트엔드 타입을 검사하고 빌드 캐시를 정리합니다.
2. `cd ~/Desktop/week2 && web-server/.venv/Scripts/python -m pytest web-server/tests -v 2>&1 | tail -20`을 실행하여 백엔드 테스트를 수행합니다.