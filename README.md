# MyZoom
줌 클론코딩 프로젝트   
<br>

## 개발환경 세팅
IDE는 Visual Studio Code 사용

1. Node.JS 설치   
   https://nodejs.org/en/ (2024-08-17 기준 v20.16.0 설치함)
2. 패키지 의존성 명시 파일 (package.json) 추가
   - npm init -y
3. Nodemon 설치
   - nodemon.json 파일 추가
     내용은 아래와 같이 세팅
      <pre>
      {
         "exec": "babel-node src/server.js"
      }
      </pre>
   - npm i nodemon -D
4. Babel 설치
   - babel.config.json 파일 추가
     내용은 아래와 같이 세팅
      <pre>
      {
         "presets": ["@babel/preset-env"]
      }
      </pre>
   - npm i @babel/core @babel/cli @babel/node @babel/preset-env -D
5. package.json에 아래 항목 추가
   - nodemon을 실행하기 위해 추가
      <pre>
      "scripts": {
         "dev": "nodemon"
      }
   </pre>
6. ExpressJS 설치
   - npm i express
7. Pug 설치
   - npm i pug
8. 프로젝트 구조 설정
   - src 디렉토리 추가
   - src/server.js 추가   
      내용을 아래와 같이 입력
      <pre>
      import express from "express";
      const app = express();
      console.log("hello");
      app.listen(3000);
      </pre>
9. 실행 테스트
   - npm run dev