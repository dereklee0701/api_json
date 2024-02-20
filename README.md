
# 1
server.js 파일 생성 
    const jsonServer = require("json-server");
    const server = jsonServer.create();
    const router = jsonServer.router("db.json");
    const middlewares = jsonServer.defaults();

    server.use(middlewares);
    server.use(router);
    server.listen(8002, () => {
    console.log("JSON Server is running");
    });

# 2
package.json 파일 생성 
    {
        "name": "react-json-server",
        "version": "1.0.0",
        "description": "",
        "main": "index.js",
        "scripts": {
            "start": "node server.js",
            "test": "echo \"Error: no test specified\" && exit 1"
        },
        "devDependencies": {
            "json-server": "^0.17.4"
        },
        "keywords": [],
        "author": "",
        "license": "ISC"
    } 

# 3 
db.json 파일 생성 및 데이터 만들기

# 4
npm install json-server

# 5
npm run start