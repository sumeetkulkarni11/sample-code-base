# springboot-websocket-stomp-chat

A **Spring Boot 3** WebSocket app using **STOMP over SockJS** with a simple **chat room** UI.

## Features
- STOMP endpoint at `/ws` with SockJS fallback
- App destinations under `/app` (e.g., `/app/chat.send`)
- Broker destinations under `/topic` (e.g., `/topic/public`)
- Minimal HTML client using SockJS + Stomp.js

## Run
```bash
mvn spring-boot:run
```
Open http://localhost:8080/ in two browser tabs to see messages broadcast in real time.

## Endpoints
- STOMP endpoint: `ws://localhost:8080/ws` (with SockJS fallback at `/ws`)
- Send messages to: `/app/chat.send`
- Subscribe to: `/topic/public`
