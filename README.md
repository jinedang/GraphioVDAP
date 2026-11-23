# Graphio VDAP 웹앱 (데모)

상단 6개 탭(홈 · 앱 카탈로그 · Studio · 템플릿 · 데이터 · 관리)과 탭별 왼쪽 세부 메뉴로 구성한 Graphio VDAP 웹앱 데모입니다.
빌드 과정 없이 `index.html` 한 파일로 동작합니다.

## GitHub Pages로 배포하기

1. 이 폴더의 파일(`index.html`, `README.md`, `.nojekyll`)을 저장소 최상위에 올립니다.
   ```
   git init
   git add .
   git commit -m "Graphio VDAP 웹앱 데모"
   git branch -M main
   git remote add origin https://github.com/newyaer89-rgb/bub.git
   git push -u origin main
   ```
2. 저장소 Settings → Pages → Build and deployment에서 Source를 `Deploy from a branch`, Branch를 `main` / `/ (root)`로 저장합니다.
3. 1~2분 뒤 `https://newyaer89-rgb.github.io/bub/` 주소로 열립니다.

특정 화면으로 바로 보내려면 주소 뒤에 `#탭-메뉴`를 붙입니다. 예: `#studio-weekly`, `#admin-urls`, `#catalog-reports`.

## 데모 계정

로그인 버튼에서 고릅니다.

| 계정 | 역할 | 할 수 있는 일 |
|---|---|---|
| 김현업 | 메이커 | 보고서 등록, Studio 생성, 승인 요청, 내 앱 관리 |
| 박이용 | 이용자 | 앱 열람, 메모 |
| 최관리 | 관리자 | 승인·반려, 전체 앱의 URL·권한·환경변수 관리 |

## 참고

- 화면의 앱·데이터·사람 이름은 모두 예시입니다.
- 메모, 승인 처리, 등록한 앱은 보는 사람의 브라우저(localStorage)에만 저장되어 다른 사람과 공유되지 않습니다.
- 앱 카탈로그 구성은 LinkaiReport(https://devreport.linkaidata.com/) v1.3.11 화면을 기준으로 옮겼습니다.
