# jjr-jonggangye-2026 — 기도로 잇고, 예배로 피어나다

중종로공동체 종강예배 & 릴레이 기도 초청 앱.

- **주소**: https://cgn210-alt.github.io/jjr-jonggangye-2026/

## 파일 구성

- `index.html` — 메인 앱 (초청장, 릴레이 기도, 참석 응답, 기도 촛불, 격려의 벽 등)
- `setup-guide.html` — 백엔드(Google Apps Script) 설정 가이드
- `worship.mp3` — 페이지 내 배경음악 파일

## 백엔드

Google Apps Script + Google 스프레드시트를 사용합니다. `index.html` 상단의 `CONFIG.APPS_SCRIPT_URL`에 배포 주소가 설정되어 있습니다. 설정 방법은 `setup-guide.html` 참고.

`index.html`은 인원수/순 개수 데이터를 [jjr-org](https://github.com/cgn210-alt/jjr-org) 저장소의 `community-totals.js`에서 가져옵니다 (공식 인원 데이터의 단일 출처는 jjr-org 쪽에 있습니다).

## 배포

`사이트-올리기.bat` 더블클릭 → `git add / commit / push` 자동 실행 → GitHub Actions가 1~2분 내 자동 배포.

## 관련 저장소

중종로공동체의 다른 프로젝트는 각각 독립된 저장소로 분리되어 있습니다.

- [jjr-org](https://github.com/cgn210-alt/jjr-org) — 조직도 / 다락방별 명단
- [jjr-baecharyo](https://github.com/cgn210-alt/jjr-baecharyo) — 조문 차량 배차표
- [jjr-sunmoim](https://github.com/cgn210-alt/jjr-sunmoim) — 순모임 주보
- [jjr-sarabat2026](https://github.com/cgn210-alt/jjr-sarabat2026) — 2026 사르밧 프로젝트(쌀 나눔)
