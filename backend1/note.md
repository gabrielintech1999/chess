1- npm init -y
2- npm install typescript --save-dev
3- npx tsc --init
4- mudar no tsconfig.json para  "outDir": "./dist",    
5- mudar no tsconfig.json par    "rootDir": "./src", 

6- npm i ws



7- put this code: 

import { WebSocketServer } from 'ws';

const wss = new WebSocketServer({ port: 8080 });

wss.on('connection', function connection(ws) {
  ws.on('error', console.error);

  ws.on('message', function message(data) {
    console.log('received: %s', data);
  });

  ws.send('something');
});




8- npm i @types/ws to ws with ts

9- npx tsc -b

10- node dist/index.js

11- Go to https://hoppscotch.io/realtime/websocket to test the server

12- create a GameManager.ts
12- create a Game.ts
12- create a message.ts