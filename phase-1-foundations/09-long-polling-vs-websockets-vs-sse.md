# Long Polling vs WebSockets vs SSE

## Diagram
```
LONG POLLING
CLIENT ──► "update?" ──► SERVER
       ◄── "YES!" ───────

WEBSOCKET
CLIENT ◄══ two way ══► SERVER

SSE
CLIENT ◄══ one way ══ SERVER
```

## Interview Questions

**Q1. What is long polling?**
> "Long polling is where client sends request and server holds it until new data is available. Once replied, client immediately asks again. Simulates real time but inefficient due to repeated connections."

**Q2. What is WebSocket?**
> "WebSocket provides a persistent two way connection between client and server. Both can send messages anytime without opening new connections. Ideal for chat apps, gaming and live collaboration."

**Q3. What is SSE?**
> "SSE stands for Server Sent Events. One way persistent connection where only server pushes updates to client. Simpler than WebSocket. Ideal for live feeds, notifications and stock prices."

**Q4. What is the difference between WebSocket and SSE?**
> "WebSocket is two way — both client and server can send. SSE is one way — only server sends. WebSocket for interactive real time apps. SSE for read only real time updates."

**Q5. When would you use each in system design?**
> "Long polling as last resort fallback. WebSocket for chat, gaming and live collaboration. SSE for live dashboards, stock tickers and notifications where only server pushes updates."

**Q6. What are disadvantages of long polling?**
> "Creates new HTTP connection every request — expensive. Adds unnecessary server load, increases latency and is inefficient at scale. Was a workaround before WebSocket existed."
