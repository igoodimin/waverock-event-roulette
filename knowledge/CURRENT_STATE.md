# 현재 상태 (2026-11-11)

## 완료
- 돌림판 기능 전체 구현, GitHub 저장소에 올림
  - https://github.com/igoodimin/waverock-event-roulette (브랜치 main)
- 2026-11-11 저장소를 공개로 바꾸고 GitHub Pages를 켬
  - 주소: https://igoodimin.github.io/waverock-event-roulette/
  - 디자인 툴 사이트(waverock-design-tools)의 보관용 칸, 강습 달력 옆에 카드 추가
- 확인함: 30명 1명 추첨, 130명 3명 추첨, 4:5·9:16 MP4 동시 저장(H.264 + AAC)
- 확인함: 20만 회 모의 실험으로 시작 위치와 당첨 결과가 무관함
- 고침: 조용한 구간이 녹음에서 빠져 소리가 앞당겨지던 문제
  - 녹음 전용으로 들리지 않는 40Hz 소리를 계속 흘려 해결(`initAudio`)
  - 소리만 따로 녹음하는 시험으로만 확인함

## 미확인
- 회전 시간을 길게(16초) 한 상태로 영상 전체를 녹화해 소리 싱크 확인 — 미리보기 창이 숨겨져 있어 못 함
- 배경 사진을 넣은 상태로 영상 저장
- 실제 인스타 업로드

## 알려진 위험
- 녹화 중 다른 탭으로 옮기면 화면 그리기(requestAnimationFrame)가 멈춰 영상이 끊긴다.
- 두 비율을 같이 저장하면 크롬이 "여러 파일 다운로드 허용"을 묻는다.

## 실행·검증 방법
- 실행: `index.html`을 크롬으로 연다. 또는 폴더에서 `python3 -m http.server 8765` 후 http://localhost:8765
- GitHub 올리기: `git push` (토큰은 Mac 키체인에 저장됨, 90일 만료 예정)

## 다음 작업
- 위 미확인 항목을 실제 크롬에서 확인한다.
