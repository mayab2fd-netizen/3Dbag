# LUMIÈRE - Premium 3D Bag Shop

프리미엄 3D 가방 쇼핑 웹사이트입니다. Three.js를 활용한 3D 가방 시각화와 AI 스타일리스트 기능을 제공합니다.

## 🚀 시작하기

### 로컬 서버 실행

브라우저 보안 정책(CORS)으로 인해 로컬 서버가 필요합니다.

```bash
# Python 3
python -m http.server 8000

# 또는 Python 2
python -m SimpleHTTPServer 8000
```

서버 실행 후 브라우저에서 다음 주소 접속:
```
http://localhost:8000/lumi_re_premium_3d_bag_shop.html
```

## 📁 프로젝트 구조

```
c:/여름학기/가방/
├── lumi_re_premium_3d_bag_shop.html  # 메인 HTML 파일
├── models/                            # 3D 모델 폴더
│   └── sample.glb                    # 가방 3D 모델
└── README.md                          # 프로젝트 설명
```

## ✨ 주요 기능

### 1. 3D 가방 쇼케이스
- Three.js 기반 3D 가방 시각화
- 드래그하여 360도 회전 가능
- 실시간 색상 변경 (코냑, 블랙, 아이보리, 세이지, 버건디)
- 자동 회전 애니메이션

### 2. 인기 상품 컬렉션
- 수평 슬라이더 형태 상품 목록
- '더보기' 버튼으로 추가 상품 로드
- AI 스타일리스트 코디 문의 기능

### 3. AI 스타일리스트
- Gemini 3 Flash 기반 멀티모달 챗봇
- 착장 사진 업로드 가능
- 스타일 추천 및 가죽 관리법 제공

## 🎨 기술 스택

- **HTML5** - 마크업
- **Tailwind CSS** - 스타일링 (CDN)
- **Three.js** - 3D 그래픽 (CDN)
- **FontAwesome** - 아이콘 (CDN)
- **Google Fonts** - 폰트 (Plus Jakarta Sans)

## 📦 3D 모델 추가 방법

새로운 3D 모델을 추가하려면:

1. `.glb` 또는 `.gltf` 형식의 3D 파일 준비
2. `models/` 폴더에 파일 배치
3. HTML 파일에서 파일명 수정:
   ```javascript
   loader.load('models/your-model.glb', function(gltf) {
       // ...
   });
   ```

## 🎨 색상 커스터마이징

가방 색상 팔레트를 수정하려면 HTML의 색상 버튼 부분을 변경하세요:

```html
<button onclick="changeBagColor(0x783e1e, 'Rich Cognac Leather')" ...>
```

## 🔧 브라우저 호환성

- Chrome/Edge (권장)
- Firefox
- Safari
- 최신 브라우저 필요

## 📝 라이선스

이 프로젝트는 개인/교육 목적으로 사용할 수 있습니다.

## 👥 협업

- 기획자: 디자인 및 UX 기획
- 디자이너: 비주얼 디자인
- 개발자: 프론트엔드 개발

---

**LUMIÈRE** - AI Integrated Premium Bag Shop
