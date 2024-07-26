# Clone Coding ZOOM

#### Requirements
- Node JS 
    - an open source and cross-platform runtime env for executing JS outside of a browser

- npm - Node Package Manager --> to install modules
    - Express (web framework)

- VanilaJS
    - creating / removing from HTML

#### Steps
##### 1. Server Setup
   1. execute command npm init -y in the terminal :- package.json should be created
   2. execute command npm install nodemon -D in the terminal to download the package
   3. execute command touch babel.config.json to create babel.config.json file
   4. open babel.config.json, babel.config.json should be {"presets": ["@babel/preset-env"]}
   5. execute command touch nodemon.json to create nodemon.json file
   6. open nodemon.json, nodemon.json should be {"exec": "babel-node src/server.js"}
   7. execute command mkdir src to create a src folder
   8. execute command cd src to change directory to src
   9. execute command touch server.js to create server.js file
  10. open server.js, server.js should be\n
       import express from "express";\n
       const app = express();\n
       app.listen(3000);
  11. execute command npm install @babel/core @babel/cli @babel/node -D @babel/preset-env -D
  12. execute command npm install express
  13. execute command npm install pug
  14. execute command npm run dev to confirm if the setup is all correct

  - optional : execute command touch README.md to add README

#### Appendix
- HTTP method
    - get request -> 주소창에서 데이터를 넘기는 방식
    - post request -> 내부적으로 body 에 정보를 담아서 요청을 보내는 방식 | 주소창 X

- 백앤드 개발 --> 프론트앤드 (UI) 에서 보낸 request 를 받아서 process 후 response 를 보내는 로직 개발