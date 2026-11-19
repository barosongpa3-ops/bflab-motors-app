BFLAB MOTORS PWA 1단계 (통합 접속 런처)

현재 범위:
- 기사용 / 정비사용 선택
- PWA 설치용 manifest, 아이콘, service worker
- 선택 시 기존 Apps Script 웹앱 주소로 이동
- 기존 구글시트/Apps Script 수정 없음

아직 미구현:
- 통합 인증 / 자동 로그인 / 외부 PWA 내 업무 화면 직접 표시
- 서버 API 연동, 관리자 세션 처리
- 이 버전은 화면 선택 후 외부 기존 웹앱으로 이동하므로 앱 안에서 업무 화면이 계속 표시되는 완전한 통합 앱은 아닙니다.

설치 순서:
1. config.js의 rider, staff에 각 운영 Apps Script 웹앱 /exec 주소 입력
2. GitHub 저장소 생성 후 이 폴더 안 파일을 저장소 루트에 업로드
3. Settings > Pages > Deploy from a branch > main / (root) > Save
4. 공개된 HTTPS 주소에서 앱 열기
5. 갤럭시 Chrome: 메뉴 > 홈 화면에 추가 또는 앱 설치
   아이폰 Safari: 공유 > 홈 화면에 추가

주의:
- GitHub Pages 공개 저장소에는 고객 정보, 시트 ID, 인증키, PIN, 구글시트 데이터, Apps Script 서버 코드를 업로드하지 마세요.
- config.js의 URL은 공개됩니다. 직원 인증은 기존 Apps Script에서 반드시 검사해야 합니다.
- 기존 Apps Script 배포 설정을 임의로 변경하지 마세요.
- 서비스워커는 정적 앱 화면만 캐시합니다. 접수/정산은 오프라인 처리되지 않습니다.
- 무료 호스팅과 설치 가능 여부는 사용 브라우저/호스팅 정책에 따라 달라질 수 있습니다.
