---
name: run-full-suite-verification
description: 프런트엔드 타입 검사와 백엔드 단위 테스트를 함께 실행하여 프로젝트 전체의 안정성을 확인합니다.
---

1. 'cd ~/Desktop/week2/frontend && npx tsc --noEmit 2>&1 | tail -30; rm -f tsconfig.tsbuildinfo'를 실행해 프런트엔드 타입 오류를 검사합니다.
2. 'cd ~/Desktop/week2 && web-server/.venv/Scripts/python -m pytest web-server/tests -v'를 실행하여 백엔드 테스트를 수행합니다.