# Agent_demo

OpenClaw + SuperGemma4 로컬 AI 에이전트 데모 레포지토리입니다.
- OpenClaw: https://github.com/openclaw/openclaw
- SuperGemma4: https://huggingface.co/Jiunsong/supergemma4-26b-uncensored-mlx-4bit-v2

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

## 🧠 OpenClaw Memory 구조

이 프로젝트는 OpenClaw의 지속적인 학습과 기억을 위해 다음과 같은 구조를 사용합니다:

- **`MEMORY.md`**: 에이전트의 핵심적인 장기 기억(Long-term memory)입니다. 중요한 결정, 학습한 교훈, 핵심적인 맥락을 담습니다.
- **`memory/YYYY-MM-DD.md`**: 매일의 작업 기록과 로그를 담는 일일 기록(Daily logs)입니다.
- **기타 컨텍스트 파일**: `AGENTS.md`, `SOUL.md`, `USER.md`, `TOOLS.md`, `IDENTITY.md` 등을 통해 에이전트의 정체성과 작업 환경을 유지합니다.
