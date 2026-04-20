# Agent_demo

OpenClaw + SuperGemma4 로컬 AI 에이전트 데모 레포지토리입니다.

## 데모 목록

### `index.html` — 오늘의 AI 기술 뉴스
- Hacker News API에서 AI/LLM 관련 뉴스를 실시간으로 가져옵니다
- 카테고리 필터: 전체 / LLM / Agent / 오픈소스 / 연구
- 별도 서버 없이 브라우저에서 바로 열 수 있습니다

## 실행 방법

```bash
open index.html
```

또는 로컬 서버로 실행:

```bash
python3 -m http.server 3000
# http://localhost:3000
```

## 연동 구성

```
GitHub (이 레포) → OpenClaw MCP → SuperGemma4 → Telegram 알림
```

- PR 생성/코드 변경 시 OpenClaw가 자동으로 감지하고 텔레그램으로 알림
- 텔레그램에서 PR 번호를 보내면 SuperGemma4가 코드 리뷰 수행
