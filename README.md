# Crypto-Agent — Design Mockups

BlueNode 개발팀 · Crypto-Agent (블록체인 학회 보조 AI Agent) 디자인 시안.

> 기획/요구사항 정의 단계 산출물. 디자인 시스템: **open-design `linear-app`** (dark-native · Inter cv01/ss03 · indigo accent). 데모 마일스톤: KBW 2026.09.

## 파일

| 파일 | 내용 |
|---|---|
| `app.html` | **전체 화면 통합 프로토타입** — 좌측 레일로 화면 전환. 대시보드 · A 학습코치 · B 코드리뷰 · C 트랜잭션설명 · H 해커톤 · 세션&노트 · 설정. 모든 Sub-Agent 풀 피델리티(다턴 대화 + 이해 캔버스 누적). |
| `index.html` | C안 단독 풀 인터랙티브 시안 (트랜잭션 한국어 설명) |
| `brief.html` | 아키텍처 → 첫 화면 → C안 1장 브리프 |

## 컨셉

채팅으로 모든 걸 끝내는 단일 AI Agent. 메인 오케스트레이터가 의도를 라우팅해 Sub-Agent(A/B/C/H)를 호출하고, 채팅 + 이해 캔버스로 한국어·출처 기반 결과를 점진 전달.

- **B 코드리뷰**: 취약점 요약 = CodeRabbit 코멘트 스타일, High 상세·수정 = GitHub *Files changed* diff 뷰 (인라인 리뷰 + 적용형 suggestion).
- 정적 HTML, 빌드 불필요. 브라우저로 바로 열기.

## 보기

각 `.html` 을 브라우저로 직접 열거나, 로컬 정적 서버:

```bash
python3 -m http.server 4173
# http://127.0.0.1:4173/app.html
```
