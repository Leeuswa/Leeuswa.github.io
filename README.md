# leeuswa.dev — 개발자 포트폴리오

백엔드 개발자 이수환의 포트폴리오 웹사이트입니다.
프레임워크나 빌드 도구 없이 **순수 HTML/CSS/JavaScript**로 제작하여 GitHub Pages로 배포했습니다.

🔗 **Live**: https://leeuswa.github.io/

---

## 구성

```text
├── index.html               메인 페이지 (소개·기술스택·프로젝트·경력·자격증·연락처)
├── projects/
│   ├── petmilyday.html      펫밀리데이 프로젝트 상세 페이지
│   └── lms.html             LMS 프로젝트 상세 페이지
├── styles.css               전체 스타일 (CSS 변수 기반 디자인 토큰)
└── favicon.svg
```

---

## 기술적 특징

- **의존성 없는 정적 사이트** — 번들러·프레임워크 없이 HTML/CSS/Vanilla JS로만 구성해 로딩이 빠르고 유지보수가 단순합니다.
- **CSS 커스텀 프로퍼티 기반 디자인 토큰** — 색상·폰트·간격을 `:root` 변수로 관리해 테마 일관성을 유지합니다.
- **IntersectionObserver 스크롤 애니메이션** — 스크롤 이벤트 리스너 대신 옵저버를 사용해 성능 부담 없이 섹션 등장 효과를 구현했습니다.
- **접근성 고려**
  - `prefers-reduced-motion` 미디어 쿼리 대응 (모션 최소화 설정 시 애니메이션 비활성화)
  - `:focus-visible` 포커스 스타일, `aria-live` 적용
- **SEO / 공유 최적화** — Open Graph 메타 태그, 페이지별 description 설정
- **반응형 레이아웃** — 모바일 내비게이션, Grid `auto-fit` 기반 카드 배치

---

## 로컬에서 보기

정적 사이트이므로 별도 빌드 과정이 없습니다.

```bash
git clone https://github.com/Leeuswa/Leeuswa.github.io.git
cd Leeuswa.github.io
# 브라우저로 index.html 열기 또는
python3 -m http.server 8000   # http://localhost:8000
```

---

## 배포

`main` 브랜치 푸시 시 GitHub Pages로 자동 배포됩니다.
