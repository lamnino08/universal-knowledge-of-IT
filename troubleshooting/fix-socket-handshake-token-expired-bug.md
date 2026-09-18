# Fix Socket Handshake Token Expired Bug

**Category:** troubleshooting
**Type:** Continuous Self-Learning Pattern
**Recorded At:** 2026-09-17

## 🔍 Problem / Context
Socket client reconnect loop occurs when auth cookie token is expired during WebSocket upgrade handshake.

## 💡 Solution & Implementation
Intercept handshake in SocketServer.ts and return explicit 401 unauthenticated error code to trigger client token refresh.

## ⚠️ Anti-Patterns / Pitfalls
Do not silently drop socket connections without emitting error event.

## 📂 Related Files
- `workspace/back-end/src/socket/SocketServer.ts`

