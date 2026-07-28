# LUMIÈRE — Premium 3D Bag Shop

> 프리미엄 가죽 가방 브랜드 **LUMIÈRE**의 쇼핑 웹사이트입니다.  
> Three.js 기반 3D 인터랙티브 뷰어, 실시간 장바구니, 모바일 최적화 UI를 제공합니다.

---

## 🚀 빠른 시작

HTML 파일을 브라우저에서 바로 열면 됩니다.

```
index.html
```

> CORS 관련 이슈가 발생할 경우 로컬 서버를 사용하세요.

```bash
# Python 3
python -m http.server 8000
# 접속: http://localhost:8000/index.html
```

---

## 📁 프로젝트 구조

```
3Dbag/
├── index.html                         # 메인 단일 파일 (HTML + CSS + JS)
├── models/
│   └── sample.glb                     # 3D 모델 샘플
└── README.md
```

---

## ✨ 주요 기능

### 🎡 3D 가방 쇼케이스
- **Three.js** 기반 3D 가방 실시간 렌더링
- 마우스 드래그 / 터치로 360° 자유 회전
- 자동 회전 애니메이션 (드래그 중 일시 정지)
- **실시간 컬러 변경** — 5가지 가죽 색상 선택 가능
  - Rich Cognac Leather
  - Midnight Obsidian Black
  - Ivory Cream Soft Leather
  - Sage Olive Green
  - Deep Burgundy

### 📖 AI 가방 스토리
- 3D 뷰어 하단 **"AI 가방 스토리 보기"** 버튼
- 선택한 컬러에 맞는 가방 스토리 텍스트 모달 팝업
- 브랜드 인용구 + 장인정신 설명

### 🛍️ 인기 상품 컬렉션
- 9개 상품 DB, 초기 6개 표시 후 **"더보기"** 로드
- 가로 슬라이더 + 좌우 화살표 스크롤
- 각 상품 카드에 **장바구니 담기** 버튼

### 🛒 장바구니
- 상품 담기 → 헤더 아이콘에 **실시간 수량 뱃지** 표시
- 우측 슬라이드 드로워로 장바구니 열기
- 수량 증감 (+/−) / 개별 삭제 / 전체 비우기
- **총 금액 실시간 합산**
- 주문하기 버튼

---

## 📱 모바일 지원

| 요소 | 모바일 최적화 내용 |
|------|------------------|
| 헤더 | 햄버거 메뉴(☰) + 사이드 내비게이션 패널 |
| 3D 뷰어 | 높이 300px(모바일) → 380px(태블릿) → 480px(데스크탑) |
| 터치 조작 | touchstart / touchmove 이벤트 완전 지원 |
| 상품 카드 | 카드 너비 220px~280px 반응형 조정 |
| 컬러 팔레트 | 가로 스크롤 지원 |

---

## 🎨 기술 스택

| 기술 | 역할 |
|------|------|
| HTML5 | 마크업 구조 |
| Vanilla CSS | 커스텀 스타일 (모달, 드로워, 애니메이션) |
| Tailwind CSS (CDN) | 유틸리티 클래스 스타일링 |
| Three.js (CDN) | 3D 가방 렌더링 |
| FontAwesome (CDN) | 아이콘 |
| Google Fonts | Plus Jakarta Sans 폰트 |
| Vanilla JavaScript | 장바구니 로직, 인터랙션 |

---

## 🎨 색상 커스터마이징

`changeBagColor()` 함수 호출로 색상을 추가할 수 있습니다.

```html
<button onclick="changeBagColor(0x783e1e, 'Rich Cognac Leather')">
```

```javascript
// 새 색상 추가 예시
changeBagColor(0x2c4a8c, 'Royal Navy Blue');
```

---

## 🔧 브라우저 호환성

- ✅ Chrome / Edge (권장)
- ✅ Firefox
- ✅ Safari
- ✅ 모바일 브라우저 (iOS Safari, Android Chrome)

---

## 📝 업데이트 이력

| 날짜 | 내용 |
|------|------|
| 2026-07-28 | 초기 버전 — 3D 뷰어, 상품 슬라이더, AI 스타일리스트 |
| 2026-07-28 | AI 스토리 텍스트 박스 모달 추가 |
| 2026-07-28 | AI 스타일리스트 기능 제거 |
| 2026-07-28 | 🛒 장바구니 기능 + 📱 모바일 반응형 개선 |

---

## 👥 팀

- **기획** — UX 기획 및 서비스 설계  
- **디자인** — 비주얼 디자인 및 브랜딩  
- **개발** — 프론트엔드 개발 (Three.js, 장바구니, 반응형)

---

**LUMIÈRE** — AI Integrated Premium Bag Shop © 2026
