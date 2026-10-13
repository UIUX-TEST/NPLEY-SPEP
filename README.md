# NPLEY × SPEP 제안서 (웹 프레젠테이션)

SPEP AI 영어 학습 앱 UX/UI 디자인 & 퍼블리싱 제안서 12장을 GSAP 전환 효과로 넘겨 보는 정적 웹 페이지입니다.

## 구성
- `index.html` — 페이지 전체(HTML·CSS·JS 한 파일). 슬라이드 데이터(`SLIDES`)가 스크립트 안에 들어 있음
- `assets/` — Figma에서 2배 해상도로 내보낸 이미지 69개 (WebP)
  - `base-NN.webp` 각 장의 본문(헤더를 뺀 배경)
  - `bg-` 큰 배경 단어 · `eye-` 아이브로 라벨 · `title-` 타이틀 · `desc-` 우측 설명 · `arrow-` 타이틀 화살표 (투명 레이어)
  - `thumb-NN.webp` 전체 보기용 썸네일
- `.nojekyll` — GitHub Pages가 Jekyll 처리하지 않도록

## 조작
←/→, 스페이스, 클릭(오른쪽 다음·왼쪽 이전), 스와이프 · G 전체 보기 · F 전체 화면 · `#s5`처럼 주소 뒤에 붙이면 해당 장으로 이동

## 외부 의존
- GSAP 3.12.5 (cdnjs) · IBM Plex Sans KR (Google Fonts, 하단 UI용)

## 원본
- Figma: https://www.figma.com/design/gKU3v3qKaXU5BWbYyvSURV (node 238:535 · Frame 2085676535)
- 슬라이드 내용을 바꾸면 Figma에서 해당 레이어를 다시 내보내 `assets/` 파일을 같은 이름으로 교체
