# KimHanbyul2000.github.io

김한별(Kim Hanbyul)의 개인 사이트 — https://kimhanbyul2000.github.io

KIST TACO Lab에서 소뇌 회로를 스파이킹 신경망(SNN)으로 모델링하고, 뉴로모픽 하드웨어로 이어지는 연산 원리를 연구합니다.

## 구성

| 경로 | 내용 |
|---|---|
| `index.html` | 메인 페이지 (소개 · 연구 · 발표자료 · 프로젝트 · 링크). 한/영 전환, 라이트/다크 테마 |
| `css/style.css` | 공통 스타일 (메인 페이지 · 발표자료가 함께 사용) |
| `favicon.svg` | 사이트 아이콘 (활동전위 파형) |
| `slides/_template/` | 발표자료 템플릿 |

같은 도메인의 하위 경로로 다른 저장소의 사이트가 연결됩니다.

- `/CV_Portfolio/` — 커리어 포트폴리오 ([CV_Portfolio](https://github.com/KimHanbyul2000/CV_Portfolio))
- `/ai-research-harness/` — [ai-research-harness](https://github.com/KimHanbyul2000/ai-research-harness)

테마(`theme`)와 언어(`lang`) 설정은 브라우저 저장소를 통해 `/CV_Portfolio/`와 공유됩니다.

## 발표자료 추가

1. `slides/_template/`을 `slides/YYYY-주제/`로 복사해 내용을 채웁니다.
2. `index.html`의 Slides 절에 있는 주석 예시대로 카드를 추가하고, "발표자료가 곧 추가됩니다" 문구를 지웁니다.
3. 문구는 한/영 쌍(`<span lang="ko">` · `<span lang="en">`)으로 넣습니다. 한쪽만 넣으면 다른 언어에서 빈칸이 됩니다.

## 로컬에서 보기

```bash
python3 -m http.server 8000   # → http://localhost:8000/
```

하단의 "마지막 업데이트" 날짜는 GitHub API로 기본 브랜치의 최신 커밋 날짜를 읽어 표시합니다(실패하면 `index.html`에 적힌 날짜).
