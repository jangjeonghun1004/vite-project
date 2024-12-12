# github pages(Vite + React)

    1. vite.config.js
        base: "/vite-project" 추가
        vite-project = github 리파지토리 네임.

    2. package.json
        "homepage": "https://jangjeonghun1004.github.io/vite-project" 추가

    3. 폴더 및 파일 생성
        ".github/workflows" 폴더 생성
        "deploy.yml" 파일 추가

    4. deploy.yml
        파일 내용을 복사해서 붙여 넣는다.

    5. github 설정
        github -> settings -> pages -> Source -> GitHub Actions 로 전한.

    

     npm install gh-pages
     "scripts": {
        "dev": "vite",
        "build": "vite build",
        "lint": "eslint .",
        "preview": "vite preview",
        "predeploy": "npm run build",
        "deploy": "gh-pages -d dist"
    },