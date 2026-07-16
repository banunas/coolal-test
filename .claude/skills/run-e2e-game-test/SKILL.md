---
name: run-e2e-game-test
description: 게임 기능 테스트를 위해 서버 상태를 확인하고 테스트 스크립트를 실행하는 단계입니다.
---

1. `source venv/bin/activate && python manage.py test game.tests -v 1 2>&1 | tail -40`으로 전체적인 테스트 로그 확인
2. 상세 확인이 필요할 경우 `tail -15`를 적용한 테스트 명령어 실행
3. 결과에 따라 필요한 데이터베이스 마이그레이션 또는 추가 확인 진행