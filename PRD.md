# Color Selector Component - PRD

## 📌 목적
사용자가 상품의 다양한 컬러 옵션 중 원하는 색상을 선택할 수 있도록 하는 컬러 선택 UI 컴포넌트. 다양한 그룹핑 옵션을 통해 사용자의 니즈에 맞는 색상 선택을 지원함.

## 👩‍💻 대상 사용자
- 의류/가구/화장품 등 색상 선택이 중요한 상품의 쇼핑몰 사용자

## 🎯 핵심 기능
- 총 30가지 색상 옵션 표시 (각 그룹핑 옵션별로 30개씩 구성)
- 원형 컬러 버튼을 클릭 시 해당 색상이 선택되고, 상단에 색상명이 표시됨
- 현재 선택된 색상은 테두리 강조로 시각적 피드백 제공
- 기본 선택값은 "Red Merlot"
- 10가지 다양한 그룹핑 옵션 제공

## 🧩 컴포넌트 구조
- `selectedColor` : 현재 선택된 색상명 표시 영역
- `colorCategories` : 3개 카테고리로 구분된 색상 표시 영역
- 각 색상은 `color-circle` 클래스를 갖는 원형 div로 표현됨

## 🎨 그룹핑 옵션

### 1. As-is (기본)
- 원본 색상 배열 그대로 표시
- Horizontal scroll 형태로 모든 색상 표시

### 2. Dark to Light (어두운색상에서 밝은색상으로)
- Dark (10개): Black, Charcoal, Navy, Steel Blue, Chocolate, Garnet, Red Merlot, Brown, Plum, Olive Green
- Medium (10개): Ash, Stone Gray, Warm Gray, Taupe, Camel, Sage Green, Blue, Green, Teal, Crimson
- Light (10개): Gold, Sand Beige, Oatmeal Beige, Dusty Blue, Sky Gray Blue, Lavender, Rose, Cream, Silver, Pearl, Ivory, White

### 3. Personal Color (퍼스널 컬러)
- Warm Tone (10개): Gold, Camel, Sand Beige, Oatmeal Beige, Warm Gray, Brown, Chocolate, Red Merlot, Garnet, Crimson
- Cool Tone (10개): Navy, Steel Blue, Blue, Dusty Blue, Sky Gray Blue, Green, Sage Green, Olive Green, Teal, Lavender
- Neutral Tone (10개): Black, Charcoal, Ash, Stone Gray, Taupe, Ivory, Cream, Pearl, Silver, White

### 4. Color Tone (컬러 톤)
- Bright (10개): Gold, Blue, Green, Teal, Crimson, Lavender, Rose, Dusty Blue, Sky Gray Blue, Sage Green
- Pastel (10개): Ivory, Cream, Pearl, Silver, White, Oatmeal Beige, Sand Beige, Warm Gray, Stone Gray, Taupe
- Natural (10개): Black, Charcoal, Ash, Navy, Steel Blue, Camel, Brown, Chocolate, Red Merlot, Garnet, Plum, Olive Green

### 5. Tone & Saturation (톤·채도 기반)
- Light Tone (10개): Ivory, Cream, Pearl, White, Silver, Oatmeal Beige, Sand Beige, Dusty Blue, Sky Gray Blue, Rose
- Middle Tone (10개): Warm Gray, Stone Gray, Taupe, Camel, Sage Green, Olive Green, Blue, Green, Teal, Lavender
- Deep Tone (10개): Black, Charcoal, Navy, Steel Blue, Brown, Chocolate, Red Merlot, Garnet, Crimson, Plum

### 6. Season (시즌/컬렉션 기반)
- Spring/Summer (10개): Ivory, Cream, White, Sky Gray Blue, Dusty Blue, Lavender, Rose, Sage Green, Teal, Blue
- Fall/Winter (10개): Black, Charcoal, Navy, Steel Blue, Brown, Chocolate, Red Merlot, Garnet, Crimson, Plum
- All Season (10개): Gold, Camel, Sand Beige, Oatmeal Beige, Warm Gray, Stone Gray, Taupe, Ash, Pearl, Silver

### 7. Bestseller vs New (베스트셀러 vs 신상)
- Steady Seller (10개): Black, Navy, Charcoal, Ash, Stone Gray, Warm Gray, Ivory, Cream, White, Pearl
- New Season (10개): Gold, Crimson, Lavender, Rose, Teal, Sage Green, Dusty Blue, Sky Gray Blue, Red Merlot, Plum
- Limited Edition (10개): Camel, Sand Beige, Oatmeal Beige, Taupe, Brown, Chocolate, Garnet, Steel Blue, Green, Blue, Olive Green

### 8. Styling Purpose (스타일링 목적별)
- Base Color (10개): Black, Navy, Charcoal, Ash, Stone Gray, Warm Gray, Ivory, Cream, White, Pearl
- Point Color (10개): Gold, Crimson, Lavender, Rose, Teal, Blue, Green, Red Merlot, Plum, Sage Green
- Mix & Match (10개): Camel, Sand Beige, Oatmeal Beige, Taupe, Brown, Chocolate, Garnet, Steel Blue, Dusty Blue, Sky Gray Blue, Olive Green

### 9. Natural Motif (자연 모티프)
- Earthy (10개): Camel, Sand Beige, Oatmeal Beige, Brown, Chocolate, Taupe, Warm Gray, Stone Gray, Gold, Olive Green
- Ocean (10개): Navy, Steel Blue, Blue, Dusty Blue, Sky Gray Blue, Teal, Charcoal, Ash, Pearl, Silver
- Flora (10개): Sage Green, Rose, Lavender, Green, Crimson, Red Merlot, Garnet, Plum, Ivory, Cream, White

### 10. Mood (심리·무드 기반)
- Energetic (10개): Gold, Crimson, Red Merlot, Garnet, Blue, Green, Teal, Lavender, Rose, Sage Green
- Calm & Reset (10개): Sage Green, Taupe, Dusty Blue, Sky Gray Blue, Warm Gray, Stone Gray, Ash, Ivory, Cream, Pearl
- Premium & Luxury (10개): Black, Charcoal, Navy, Steel Blue, Camel, Brown, Chocolate, Olive Green, Plum, Silver, White

## 🎨 뉴츄럴 톤 색상 정의
패션에서 자주 사용되는 뉴츄럴 톤 색상 팔레트를 기반으로 한 분류:

### 기본 뉴츄럴 톤 색상
- **Ivory** (#FFFFF0): 따뜻하고 부드러운 화이트, 기본 이너·셔츠·원피스
- **Oatmeal Beige** (#E6D8C3): 부드럽고 포근한 느낌, 니트·코트
- **Sand Beige** (#D5C4A1): 고급스러운 모래빛, 팬츠·트렌치코트
- **Taupe** (#B9A89A): 그레이+브라운 중간톤, 가방·부츠
- **Camel** (#C19A6B): 부드러운 황갈색, 코트·가죽 재킷
- **Warm Gray** (#B0A99F): 온기가 느껴지는 회색, 재킷·팬츠
- **Stone Gray** (#A49B90): 차분하고 묵직한 그레이, 셋업 수트

### 포인트 뉴츄럴 톤 색상
- **Sage Green** (#B2AC88): 허브빛 연녹색, 가디건·셔츠
- **Olive Green** (#8B8C6A): 카키보다 부드러운 톤, 야상·팬츠
- **Dusty Blue** (#A3B5C3): 채도 낮춘 파스텔 블루, 셔츠·니트
- **Sky Gray Blue** (#BCCAD6): 흐린 하늘빛, 원피스·블라우스

### 뉴츄럴 톤 특징
- 모두 채도가 낮아 서로 조합하기 쉬움
- 베이지·그레이·브라운 계열이 기본 축
- 포인트로 세이지그린·더스티블루처럼 색감이 있는 뉴츄럴톤을 섞으면 세련됨

## 🧠 인터랙션
- 클릭 시 해당 색상이 선택됨 (단일 선택)
- 선택된 색상은 `.selected` 클래스가 적용되어 테두리로 강조
- `title` 속성으로 hover 시 색상명 제공
- JavaScript를 통해 선택 이벤트 및 UI 업데이트 처리
- 각 그룹핑 옵션별로 30개씩 색상 구성

## 🛠️ 기술 스택
- HTML: 구조 구성
- CSS: 컬러 원 스타일링 및 인터랙션 효과
- JavaScript: 선택 이벤트 및 UI 상태 업데이트

## 🖼️ 향후 확장 가능성
- 선택한 색상에 따라 이미지 변경
- 품절 색상 비활성화 처리
- 다국어 대응 (색상명 번역)
- 키보드 접근성 개선 (tab/enter 지원)