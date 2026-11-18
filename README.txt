MD Studio PWA 파일 구성
- index.html: 모바일 최적화 Markdown 편집기
- manifest.json: 홈 화면 설치 정보
- sw.js: 앱 셸 오프라인 캐시
- icons/: 앱 아이콘

설치/사용 방법
1. 네 파일과 icons 폴더를 같은 웹사이트 경로에 업로드합니다.
2. HTTPS로 접속합니다. (localhost 개발 환경도 가능)
3. Android Chrome에서 메뉴(⋮) > 앱 설치 또는 홈 화면에 추가를 선택합니다.
4. 최초 접속 후 앱 셸이 캐시되면 기본 편집 화면은 오프라인에서도 열립니다.

중요
- 보안상 Android Chrome은 일반 file:// 파일을 PWA로 설치하거나 Service Worker를 실행하지 않습니다.
- 따라서 index.html을 휴대폰에서 직접 여는 것은 가능하지만, PWA 설치 및 오프라인 캐시를 사용하려면 HTTPS 웹 호스팅이 필요합니다.
- 사용자가 편집한 문서의 자동 영구 저장은 아직 포함되어 있지 않습니다. Markdown 저장 메뉴로 파일을 내려받으세요.
- PDF 내보내기는 브라우저 인쇄 기능을 사용합니다.
