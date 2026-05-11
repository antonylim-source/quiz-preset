# AI Playground — 2026년 4월 신규 게임 프로모션 페이지

초등학생을 위한 **AI 기반 교육 게임 플랫폼** 소개용 정적 랜딩 페이지입니다. **신규 게임 2종**을 카드 형태로 안내합니다.

## 페이지 열기 (로컬 파일)

브라우저 주소창에 아래 URL을 붙여 넣거나, 즐겨찾기에 저장해 두면 됩니다.

```
file:///E:/001.%20MyWork/12.%20AI%20Playground/_promotion/index.html
```

**참고:** 경로에 공백이 있어 URL에서는 `%20`으로 인코딩되어 있습니다. 탐색기에서 `index.html`을 더블클릭해도 동일하게 열립니다.

### 다른 방법

- **PowerShell** (프로젝트 폴더에서): `Start-Process .\index.html`
- **로컬 HTTP 서버**가 필요한 기능이 있다면(예: 일부 CORS 제한), `npx serve` 등으로 폴더를 띄운 뒤 해당 주소로 접속합니다.

## 포함된 콘텐츠

| 게임 | 앵커 ID | 영역(태그) | 한 줄 소개 |
|------|---------|------------|------------|
| Emoji Story Chain | `#Emoji` | Writing, Speaking (optional) | 이모지 조건 영작·AI 튜터 피드백·(선택) 음성 입력 |
| Magic Word World | `#magic-word` | Grammar, Listening, Reading | 그리스 로마 신화 퀴즈·Orb 수집·나만의 세계 이미지 생성 |

`#games` 빠른 탐색과 상단 히어로의 「게임 살펴보기」에서 각 섹션으로 스크롤 이동할 수 있습니다.

## 기술 스택

- **HTML5** 단일 파일 (`index.html`)
- **Tailwind CSS** — CDN (`https://cdn.tailwindcss.com`), `tailwind.config`로 브랜드 색·폰트 확장
- **Pretendard** — jsDelivr CDN (`pretendard.min.css`)
- **Google Fonts** — Noto Sans KR (보조)
- **Vanilla JavaScript** — `IntersectionObserver`로 스크롤 시 카드 등장(reveal) 애니메이션

인터넷 연결이 있어야 Tailwind·웹폰트가 정상 로드됩니다.

## 에셋(이미지)

`index.html` 기준으로 **`images/` 폴더** 아래 파일이 있어야 썸네일이 표시됩니다.

- `images/Emoji-Story-Chanin.jpeg` — Emoji Story Chain
- `images/Magic-Word-World.png` — Magic Word World

이미지가 없으면 브라우저에서 깨진 그림으로 보일 수 있습니다.

## 파일 구성

```
_promotion/
├── README.md      ← 이 파일
├── index.html     ← 프로모션 페이지 본문
└── images/        ← 썸네일 이미지(위 목록)
```

## 저작권 표기

페이지 푸터: © 2026 AI Playground. All rights reserved.
