---
name: run-game-migration-cycle
description: Django에서 마이그레이션 생성 후 검사 및 테스트를 수행하는 일련의 과정을 표준화합니다.
---

1. `git status`로 현재 변경 사항 확인
2. `source venv/bin/activate && python manage.py makemigrations game 2>&1` 실행
3. 필요에 따라 `python manage.py migrate game 2>&1` 또는 `python manage.py showmigrations game 2>&1`을 실행하여 상태 업데이트 및 확인