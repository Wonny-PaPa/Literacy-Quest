# 문해력 원정대 PWA (GitHub Pages)

## 배포 방법
1. 이 폴더 안의 파일과 `icons` 폴더를 GitHub 저장소 최상위(root)에 업로드합니다.
2. 저장소의 **Settings → Pages**로 이동합니다.
3. **Deploy from a branch**를 선택하고 배포 브랜치와 `/ (root)`를 지정한 뒤 저장합니다.
4. 배포가 완료되면 GitHub Pages 주소로 접속합니다. HTTPS 주소에서 앱 설치 기능을 사용할 수 있습니다.

## 파일 구성
- `index.html`: 문해력 원정대 앱 본체 및 PWA 메타 태그
- `manifest.webmanifest`: 앱 이름, 실행 방식, 화면 방향, 테마 및 아이콘 설정
- `icons/`: 브라우저·Android·iOS용 아이콘

## 참고
- GitHub Pages는 HTTPS로 제공되므로 manifest 사용 조건을 충족합니다.
- 현재 구성은 홈 화면 설치용 manifest와 아이콘을 포함합니다. 오프라인 실행 및 캐시 업데이트 기능은 별도의 Service Worker가 필요하며 이번 요청 범위에는 포함하지 않았습니다.
- 배포 경로가 저장소 하위 경로여도 상대 경로(`./`)로 manifest와 아이콘을 찾도록 구성했습니다.
