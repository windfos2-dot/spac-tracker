# SPAC Tracker

KOSDAQ 기업인수목적회사(스팩) 트래커 대시보드 — 합병 진행·공모가 괴리·합병기한·신규 상장.

**Live:** https://windfos2-dot.github.io/spac-tracker/

## 구성
- `index.html` — 대시보드 (Tailwind CDN, `spac_tracker_latest.json` 로드)
- `spac_tracker_latest.json` — 데이터 (금융위 상장종목 · KIS 시세 · OpenDART 합병공시)

## 갱신
데이터는 별도 파이프라인(`telegram_bot/spac_tracker.py`)이 생성합니다.
갱신 시 `telegram_bot/publish_spac.py` 실행 → 최신 JSON을 이 저장소로 커밋·푸시.

> 데이터 출처는 전부 공개 정보이며, 투자판단의 근거가 아닙니다. 원자료(DART·거래소) 확인 필요.
