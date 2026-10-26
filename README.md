
# 🥗 냉장고 재료 관리 & 레시피 추천 앱 (iOS)

냉장고 속 재료들의 **유통기한을 관리**하고, 그 재료가 들어가는 **레시피를 추천**해주는 iOS 앱입니다.

> 한성대학교 iOS 프로그래밍 프로젝트 · 2171438 조해리

## 🎬 시연 영상
👉 [데모 영상 보기](https://github.com/haeri-J/iosproject/releases/tag/V1.0)

## 주요 기능

### 1) 냉장고 속 음식들 (냉장고 페이지)
- 사용자가 냉장고 속 음식을 **이름, 날짜, 메모, 사진**과 함께 등록할 수 있고, **오래된 순**으로 위에 정렬됩니다.
- 유통기한을 기준으로 **과거 / 오늘 / 미래 / 전체**, 4개의 카테고리로 아이템을 나눠 보여줍니다.
- `Edit` 버튼을 누르면 아이템을 **삭제**할 수 있고, `>`를 누르면 수정 페이지로 들어가 아이템을 **수정**할 수 있습니다.
- 상단의 **달력 아이콘**을 누르면 등록한 음식의 유통기한을 달력 형태로 볼 수 있습니다.

### 2) 레시피 추천 페이지
- 리스트에 등록된 재료를 바탕으로, 그 재료가 들어가는 **레시피를 찾아 추천**합니다.
- 레시피는 **밥, 국&찌개, 일품, 반찬, 기타**, 5개의 카테고리로 나뉩니다.
- 레시피 데이터는 **식약처 오픈 API**에서 가져오며, 레시피를 누르면 **상세 레시피 페이지**가 나옵니다.

## 파일 구성

| 파일 | 역할 |
|---|---|
| `iosN_2171438_johaeriApp.swift` | 앱 진입점 |
| `ContentView.swift` | 탭 구성 (냉장고 / 레시피 추천), `FoodItems` 데이터 모델 |
| `MyListView.swift` | 냉장고 속 음식 리스트, 카테고리 분류 |
| `EditFoodItemView.swift` | 음식 등록·수정 화면 |
| `ImagePicker.swift` | 음식 사진 선택 |
| `CalendarView.swift` | 유통기한 달력 보기 |
| `RecipeRecommendationView.swift` | 재료 기반 레시피 추천 화면 |
| `RecipeDetailView.swift` | 레시피 상세 화면 |
| `RecipeManager.swift` / `RecipeData.swift` | 레시피 데이터 관리 및 모델 |
| `fetchRecipeData.swift` | 식약처 오픈 API 호출 |

## 사용 기술
- Swift / **SwiftUI** (`TabView`, `NavigationView`, `@StateObject`, `ObservableObject`)
- 식품의약품안전처 레시피 오픈 API
- Xcode, iPhone 14 Pro 시뮬레이터

## 실행 방법
1. 레포를 클론합니다.
2. `iosN_2171438_johaeri.xcodeproj`를 Xcode로 엽니다.
3. 시뮬레이터를 고르고 ▶︎ Run을 누릅니다.
