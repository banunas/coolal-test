---
name: check-git-status
description: 작업 중 변경 사항을 확인하고 검증 스크립트를 실행하는 과정입니다.
---

1. `git status --short`를 실행하여 현재 변경된 파일을 확인합니다.
2. `PYTHONPATH=/Users/banu/dev/madcamp/codebee/26s-w1-c2-06/backend ./venv/bin/python /tmp/ws_verify.py 2>&1` 명령을 실행하여 변경 사항이 정상적으로 작동하는지 검증합니다.