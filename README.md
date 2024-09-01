# MyZoom
줌 클론코딩 프로젝트
<br>

## 개발 환경 세팅
사용 IDE: Visual Studio Code

1. Node.JS 설치   
   https://nodejs.org/en/ (2024-08-17 기준 v20.16.0 설치함)
2. Nodemon 설치
   - npm i nodemon -D
3. Babel 설치
   - npm i @babel/core @babel/cli @babel/node @babel/preset-env -D
4. ExpressJS 설치
   - npm i express
5. Pug 설치
   - npm i pug
6. Socket.IO 설치
   - npm i socket.io 

## 실행 테스트
   - 서버 실행
      - npm run dev
   - 서버 Admin 페이지
      1. npm i @socket.io/admin-ui (터미널에서 설치)
      2. https://admin.socket.io 접속 후   
         Server URL: http://localhost:3000   
         Admin namespace: /admin
