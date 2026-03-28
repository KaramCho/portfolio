# Portfolio · Karam Cho

**Shopify · React · TypeScript** 프론트엔드 개발자 포트폴리오. 단일 정적 페이지로 구성되어 있으며, 빌드 도구 없이 바로 열거나 정적 호스팅에 올릴 수 있습니다.

---

## 특징

- **다크 / 라이트 테마** — 토글 + `localStorage`로 선호 저장
- **한국어 / 영어** — 상단 언어 선택 + `localStorage` 동기화
- **Tailwind CSS (CDN)** — 커스텀 토큰·다크 모드(`class`) 연동
- **접근성** — 시맨틱 마크업, `aria-label`, 스크롤 네비게이션
- **반응형** — 모바일부터 데스크톱까지 단일 레이아웃

## 기술 스택

| 영역 | 사용 |
|------|------|
| 마크업 / 스타일 | HTML5, Tailwind (Play CDN), CSS 변수 |
| 스크립트 | 바닐라 JS (i18n, 테마, 언어 초기화) |
| 폰트 | Inter, JetBrains Mono, Noto Sans KR |

## 구조

```
.
├── index.html          # 사이트 (UI · i18n · 테마)
├── README.md
├── .gitignore
├── assets/
│   └── avatar.png      # 프로필 이미지
└── docs/
    └── portfolio.md    # 영문 원문/이력 마크다운 (참고용)
```

## 로컬에서 보기

정적 파일이므로 브라우저에서 `index.html`을 열어도 됩니다. 다만 `file://` 환경에서 일부 브라우저 정책이 다를 수 있어, 아래처럼 간단한 서버를 쓰는 편이 안전합니다.

```bash
# Python 3
python3 -m http.server 8080
# → http://localhost:8080
```

## GitHub에 올리기

저장소: `git@github.com:KaramCho/portfolio.git`

```bash
cd /path/to/portfolio
git init
git add .
git commit -m "Initial commit: static portfolio"
git branch -M main
git remote add origin git@github.com:KaramCho/portfolio.git
git push -u origin main
```

**GitHub Pages**로 공개하려면 저장소 Settings → Pages → Branch를 `main` / root(또는 `/docs`)로 지정하면 됩니다.

---

## 라이선스

개인 포트폴리오용 콘텐츠입니다. 코드 재사용 시 출처를 남겨 주시면 감사하겠습니다.
