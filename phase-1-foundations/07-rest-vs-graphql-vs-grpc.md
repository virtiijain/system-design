# REST vs GraphQL vs gRPC

## Diagram
```
REST
CLIENT ── GET /users/1 ──► SERVER
       ◄── full user object ──
       (got all fields, needed only name = overfetching)

─────────────────────────────────────

GraphQL
CLIENT ── query { user { name } } ──► SERVER
       ◄── { name: "Virti" } ──
       (got exactly what was needed ✓)

─────────────────────────────────────

gRPC
SERVICE A ══ binary data ══► SERVICE B
          ◄══ response ══
          (fastest, used between microservices)
```

## 🎯 Interview Questions

**Q1. What is REST?**
> "REST is an architectural style for APIs using HTTP. Client sends requests to fixed endpoints and server returns data. Simple, widely used, easy to understand."

**Q2. What is GraphQL?**
> "GraphQL is a query language for APIs by Facebook. Client specifies exactly what data it needs — eliminates overfetching and underfetching."

**Q3. What is gRPC?**
> "gRPC is a high performance framework by Google using binary Protocol Buffers instead of JSON. 10x faster than REST. Used for server to server communication in microservices."

**Q4. What is overfetching and underfetching?**
> "Overfetching means getting more data than needed. Underfetching means one request is not enough, need multiple calls. GraphQL solves both by letting client ask for exactly what it needs."

**Q5. When to use GraphQL over REST?**
> "When frontend needs flexible data, multiple clients need different data from same API, or overfetching is causing performance issues."

**Q6. When to use gRPC over REST?**
> "For internal microservice communication where speed is critical. gRPC is 10x faster due to binary protocol. Not suitable for public APIs due to limited browser support."
