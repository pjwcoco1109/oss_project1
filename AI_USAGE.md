# 생성형 AI 사용 기록

이 과제에서 생성형 AI(ChatGPT, Claude, Gemini, Copilot 등)를 쓸 때마다 아래 표에 **한 줄씩** 추가할 것.

- **날짜**: 사용한 날 (YYYY-MM-DD)
- **도구**: 사용한 AI 도구 이름
- **관련 기능**: F1–F5 중 무엇 (Git 사용법·README 등 기능과 무관하면 `기타`)
- **무엇을 물었나**: 질문·요청 내용을 구체적으로 (예: "pygame 에서 사각형 충돌을 확인하는 함수")
- **결과를 어떻게 반영/수정했나**: 받은 답을 그대로 썼는지, 어디를 고쳤는지, 쓰지 않았다면 왜인지

AI 를 전혀 쓰지 않았다면 표를 지우고 "이 과제에서 생성형 AI 를 사용하지 않았습니다." 라고 적을 것.
아래 `예시` 줄은 지우고 제출할 것.

| 날짜 | 도구 | 관련 기능 | 무엇을 물었나 | 결과를 어떻게 반영/수정했나 |
|---|---|---|---|---|
|2026-11-15|ChatGPT|기타|커밋메시지와 브랜치 이름을 어떤 형식으로 어떻게 써야하는지 확인함|답변받은 추천메시지를 참고하여 커밋메시지와 브랜치이름을 작성함 |
|2026-11-15|ChatGPT|기타| `__pycache__/`, `*.pyc`, 가상환경, `highscore.txt`를 제외하는 `.gitignore` 파일 생성 요청 | ChatGPT가 생성해 준 `gitignore` 파일을 다운로드해 프로젝트 최상위 폴더에 넣어 사용함 |
|2026-11-15|ChatGPT|기타| `gitignore` 파일명 앞에 점(`.`)을 붙여 `.gitignore`로 변경하는 방법과 GitHub Desktop 커밋·푸시 방법 문의 | 안내받은 대로  파일명을 `.gitignore`로 수정한 뒤 GitHub Desktop에서 `chore: .gitignore 파일명 수정` 메시지로 커밋·푸시함 |
|2026-11-15|ChatGPT|F1| 플레이어가 방향키를 누르면 좌우로 이동하고 화면 밖으로 나가지 않도록 제한하는 방법 | 제공받은 코드를 그대로 사용하여 Player의 update 함수에 적용함 |
|2026-11-15|ChatGPT|F1|entities.py 실행 중 발생한 IndentationError의 원인과 해결 방법|들여쓰기 오류가 발생한 부분을 확인하고 함수 내부 코드의 들여쓰기를 수정함 |
|2026-11-15|ChatGPT|기타|main.py 실행 중 창이 바로 종료되는 문제의 원인과 확인 방법|IDLE에서 main.py를 실행하고 오류 메시지를 확인하는 방법을 참고함 |
|2026-11-15|ChatGPT|기타|과제의 AI_USAGE.md 작성 요건과 기록 방법|과제 안내문의 작성 기준을 확인하고 실제 AI 사용 내역을 정리함 |
|2026-11-15|Gemini|기타| main 브랜치에 md 파일이 먼저 올라간 상태에서 feature/move 브랜치를 --no-ff로 머지하는 방법 및 병합 상태 점검 | 안내받은 대로 main 브랜치로 이동 후 git pull origin main과 git merge --no-ff feature/move를 순서대로 실행하여 원격 저장소에 반영함 |
|2026-11-16|Gemini|F2| 플레이어 총알 생성·이동(entities.py) 및 스페이스바 발사 입력 처리(main.py) 구현 방법 | 안내받은 코드를 사용하여 Player.shoot, Bullet.update, Game.handle_events에 반영하고 실행 동작을 확인함 |
|2026-11-16|Gemini|기타| GitHub Desktop에서 feature/bullet 브랜치 커밋 후 --no-ff 머지 및 History 확인 방법 | 안내받은 대로 GitHub Desktop에서 커밋 후 터미널 명령어(git merge --no-ff)로 main에 병합함 |
|2026-11-16|Gemini|F3| 총알과 적의 충돌 판정(groupcollide) 및 화면 왼쪽 상단 점수 표시 구현 방법 | 안내받은 코드를 사용하여 Game.update와 Game.draw에 반영하고 실행 동작을 확인함 |
|2026-11-17|Gemini|F4| F4(적 충돌·화면 이탈 시 생명 감소 및 게임 오버 화면) 구현 코드를 요청하고, 코드 작성 후 발생한 들여쓰기 오류 원인과 해결 방법과 --no-ff로 머지하는 방법을 물어봄 | 제공받은 코드를 main.py(update, draw_game_over)에 적용한 뒤, 안내받은 대로 end_game과 draw_game_over의 들여쓰기 오류를 수정하고 실행 테스트 및 --no-ff 머지를 완료함 |
|2026-11-17|Gemini|F5| F5(최고 점수 파일 저장·불러오기 및 게임 오버 후 R 키 재시작) 구현 코드를 요청하고, 코드 작성 후 발생한 들여쓰기 오류 점검과 기존 주석/pass 삭제 여부와 --no-ff로 머지하는 방법을 물어봄 | 제공받은 코드를 main.py(load_high_score, save_high_score, handle_events, end_game, draw_game_over)에 적용하고, end_game 내부 if문 들여쓰기를 수정한 뒤 실행 테스트 및 --no-ff 머지를 완료함 |
|2026-11-17|Gemini|기타| README.md [학생 작성] 완료 목록 문구와 AI_USAGE.md 작성 내용을 요청하고, 메모장 마크다운 자동 변환(역슬래시) 해결법과 .gitignore 동작 여부를 확인함 | 제공받은 문구를 사용하여 README.md의 F1~F5 체크리스트를 구문 모드에서 수정·커밋하고, AI_USAGE.md에 실제 코드 요청 및 수정 내역을 기록함 |