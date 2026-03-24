# Forward Proxy vs Reverse Proxy

## Diagram
```
FORWARD PROXY
CLIENT ──► PROXY ──► SERVER
(client hidden from server)

─────────────────────────

REVERSE PROXY
CLIENT ──► PROXY ──► SERVER
(server hidden from client)
```

## Interview Questions

**Q1. What is a proxy?**
> "A proxy is a middleman between client and server. Requests go through proxy first. It can hide identity, filter requests, cache responses or distribute load."

**Q2. What is a forward proxy?**
> "Forward proxy sits in front of client. Server only sees proxy IP, not client IP. Used for anonymity, bypassing restrictions and caching. VPN is a common example."

**Q3. What is a reverse proxy?**
> "Reverse proxy sits in front of server. Client never knows which server handled request. Used for load balancing, security, caching and SSL termination. Nginx and Cloudflare are popular examples."

**Q4. What is the difference between forward and reverse proxy?**
> "Forward proxy hides client from server. Reverse proxy hides server from client. Forward proxy is client side, reverse proxy is server side."

**Q5. Why is reverse proxy important in system design?**
> "Reverse proxy is the single entry point for all requests. It distributes traffic across servers, terminates SSL, caches responses and protects servers from direct internet exposure."

**Q6. What is SSL termination?**
> "SSL termination means reverse proxy handles all HTTPS encryption and decryption. Backend servers receive plain HTTP — offloads heavy encryption work making them faster."
