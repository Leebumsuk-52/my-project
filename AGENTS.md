# 프로젝트 작업 규칙

향후 코드 작업을 시작하기 전에 이 문서와 기존 파일 및 설정을 먼저 확인하고, 필요한 부분만 수정합니다.

- 이 프로젝트는 Vanilla JavaScript를 사용하는 Vite 프로젝트입니다.
- HTML, CSS, JavaScript 코드는 각각 분리된 파일로 작성합니다.
- `index.html`은 프로젝트 루트에 둡니다.
- 애플리케이션의 CSS와 JavaScript 파일은 `src` 폴더에 작성합니다.
- `vite.config.js` 등 설정 파일은 프로젝트 루트에 둡니다.
- JavaScript는 `type="module"`로 연결합니다.
- CSS는 JavaScript 진입 파일에서 import하여 Vite 빌드에 포함합니다.
- 외부 JavaScript 라이브러리는 `npm install`로 설치하고 import하여 사용합니다. CDN 방식은 사용하지 않습니다.
- Vite의 기본 진입점인 루트 `index.html`과 기본 빌드 출력 폴더인 `dist`를 사용하며, 불필요한 설정은 추가하지 않습니다.
- 변경 후 `npm run build`로 빌드가 정상 완료되는지 확인합니다.

## GitHub 및 Netlify 배포

프로젝트를 GitHub에 업로드한 후 Netlify에서 해당 저장소를 연결합니다.

- Build command: `npm run build`
- Publish directory: `dist`

`node_modules`와 `dist`는 기존 `.gitignore` 설정에 따라 GitHub에 업로드하지 않습니다.
