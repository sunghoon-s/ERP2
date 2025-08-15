ERP Data Analyzer

간단한 브라우저 기반 엑셀(Excel) 분석 도구입니다.
- `index.html`: 엑셀 파일 업로드, 제품/공정 선택, 필터링 후 분석 데이터 전송
- `analysis_latest.html`: 전송된 데이터로 KPI/차트 요약 및 CSV 다운로드

빠른 시작
1. 로컬에서 `index.html`을 더블클릭하여 브라우저에서 엽니다.
2. 엑셀 파일(.xlsx/.xls)을 업로드합니다.
3. 제품군/공정을 선택하고 "분석 시작"을 눌러 새 창에서 분석 결과를 확인합니다.

GitHub에 올리는 방법 (PowerShell 예시)
- 로컬에서 최초로 Git 저장소를 만들고 커밋한 뒤 원격에 푸시하는 일반적인 명령입니다.

# Git이 설치되어 있어야 합니다. (https://git-scm.com/)
# 1) 저장소 초기화 및 커밋
git init ; git add . ; git commit -m "Initial commit: ERP data analyzer"

# 2) GitHub에 새 리포지토리 생성 (방법 A: gh CLI 사용)
# gh CLI가 설치되어 있고 로그인되어 있다면 아래 명령으로 새 repo를 만들고 푸시할 수 있습니다:
# gh repo create <REPO_NAME> --public --source . --remote origin --push

# 3) (방법 B: 수동) GitHub 웹에서 리포지토리 생성 후 원격 추가 및 푸시
# 예: https://github.com/<your-user>/<repo>.git 로 만들었다면
git remote add origin https://github.com/<your-user>/<repo>.git ; git branch -M main ; git push -u origin main

참고
- 브라우저에서 직접 열어 쓰는 정적 프로젝트입니다. 서버가 필요 없으며 SheetJS(CDN)를 사용합니다.
- 민감한 파일(실행 파일, 개인 토큰 등)은 커밋하지 마세요.

도움 필요하시면 원격 리포지토리 URL을 알려주거나, 제가 여기서 `git` 명령을 실행해 드리길 원하면 알려주세요. (push는 사용자의 인증/환경에 따라 동작합니다.)
