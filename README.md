# c219 - Video Chat App

A real-time multi-user video chat room app with text chat, built with Express, Socket.io and PeerJS (WebRTC).

## Features
- Unique room per session (UUID redirect from `/`).
- Live video + audio streaming between peers via PeerJS/WebRTC.
- Text chat broadcast to the room via Socket.io.
- Mute/unmute mic, show/hide video, and chat sidebar toggles.

## Tech Stack
- Node.js, Express 4, EJS
- Socket.io 4
- Peer (PeerJS server) + peerjs client
- uuid

## Project Structure
```
c219/
├── server.js         # express + socket.io + peer server
├── views/index.ejs   # room UI
├── public/
│   ├── script.js     # WebRTC/PeerJS client logic
│   └── style.css
└── package.json
```

## Installation
```
npm install
```

## Usage
```
npm start
```

Then open `http://localhost:3030` (or the `PORT` env var). You'll be redirected to a unique room URL; share it with others to chat.