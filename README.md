# maesil.net

주식회사 매실 패밀리 공식 웹사이트.

## 구조

```
.
├── index.html           # 랜딩 페이지 (제품 라인업 + 공고 링크)
├── notice/
│   └── index.html       # 상법상 공식 공고 게시 페이지 (정관 제4조)
└── README.md
```

## 배포

정적 HTML이라 별도 빌드 없이 다음 중 한 곳에 그대로 올리면 바로 서비스 가능.

- **Cloudflare Pages** (권장, 무료 + CDN + SSL 자동)
- **GitHub Pages** (리포지토리 `Settings → Pages`)
- **Netlify** (드래그앤드롭)
- **Vercel** (정적 사이트 프리셋)

배포 후 커스텀 도메인 `maesil.net` 연결 → DNS 전파 30분~2시간 내 완료.

## 공고 게시 방법

`notice/index.html`의 `<div class="empty">` 블록을 지우고 `<ul class="notice-list">` 안에 `<li>` 블록을 복사해 새 공고를 추가한다. 각 공고는 게시일로부터 **최소 5년간 유지** (상법시행령 제6조).

예시:

```html
<li>
  <div class="meta">
    <span class="category">재무제표 공고</span>
    <span>게시일: 2027-03-21</span>
    <span>공고번호: 2027-001</span>
  </div>
  <p class="title">제1기 재무제표 공고</p>
  <p class="summary">제1기(2026.4.20 ~ 2026.12.31) 대차대조표 및 손익계산서 공고</p>
</li>
```

## 법인 정보

| 항목 | 값 |
|---|---|
| 상호 | 주식회사 매실 패밀리 · MAESIL FAMILY CO., LTD. |
| 대표이사 | 김은지 |
| 설립일 | 2026년 4월 20일 |
| 본점 | 경상남도 김해시 주촌면 서부로1403번길 8-63 |
| 공고 방법 | 회사 인터넷 홈페이지(https://maesil.net) 게재 |

## 제품 라인업

- **매실 인사이트** (Maesil Insight) — 온라인 데이터 분석 SaaS · 서비스 중
- **매실 허브** (Maesil Hub) — 식품·축산 전용 ERP · 개발 중
- **매실 토탈** (Maesil Total) — 제조·물류 통합 운영 플랫폼 · 개발 중
- **매실 플로우** (Maesil Flow) — 3PL 전용 물류 관리 SaaS · 개발 중
- **매실 브랜딩** (Maesil Branding) — AI 기반 상품 상세페이지 자동 생성 · 개발 중
