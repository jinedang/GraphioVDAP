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

## 로그인

앱에 들어가려면 회사 이메일과 비밀번호로 로그인해야 합니다. 가입 화면은 없고, 관리자가 관리 › 구성원 계정에서 초대 링크(7일, 1회용)를 만들어 전달하면 사원이 그 링크에서 비밀번호를 정합니다. 비밀번호 재설정 링크(1시간, 1회용)도 관리자가 만듭니다.

데모 계정 (비밀번호 모두 `vdap1234`)

| 계정 | 역할 | 할 수 있는 일 |
|---|---|---|
| admin.choi@mobigen.example | 관리자 | 승인·반려, 구성원 초대·비활성화, 전체 앱 관리 |
| hyunup.kim@mobigen.example | 메이커 | 보고서 등록, Studio 생성, 승인 요청, 내 앱 관리 |
| iyong.park@mobigen.example | 이용자 | 앱 열람, 메모 |

초대 수락 화면 예시: 주소 끝에 `#invite-welcomeinsa7`

## 참고

- 화면의 앱·데이터·사람 이름은 모두 예시입니다.
- 계정, 비밀번호, 메모, 승인 처리, 등록한 앱은 보는 사람의 브라우저(localStorage)에만 저장되어 다른 사람과 공유되지 않습니다. 실제 회사 비밀번호를 쓰지 마세요.
- 앱 카탈로그 구성은 LinkaiReport(https://devreport.linkaidata.com/) v1.3.11 화면을 기준으로 옮겼습니다.
