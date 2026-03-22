# HTTP / HTTPS

## Diagram
```
CLIENT                        SERVER
  │                               │
  │──── HTTP REQUEST ────────────►│
  │     (GET /home)               │
  │                               │
  │◄──────────── HTTP RESPONSE ───│
  │     (200 OK + HTML page)      │
  │                               │

HTTP  = plain text (anyone can read)
HTTPS = encrypted (no one can intercept)

HTTP  → port 80
HTTPS → port 443
```

## HTTP Methods
```
GET    → fetch data
POST   → create data
PUT    → update data
DELETE → delete data
```

## HTTP Status Codes
```
200 → OK
201 → Created
301 → Redirect
400 → Bad request
401 → Unauthorized
403 → Forbidden
404 → Not found
500 → Server error
```

## Interview Questions

**Q1. What is HTTP?**
> "HTTP stands for HyperText Transfer Protocol. It is the set of rules that defines how a client and server communicate on the web — how requests are made and how responses are returned."

**Q2. What is the difference between HTTP and HTTPS?**
> "HTTP sends data as plain text — anyone in between can read it. HTTPS is the secure version — it encrypts data using SSL/TLS so no one can intercept it. Any site handling sensitive data like login or payments must use HTTPS."

**Q3. What are HTTP methods?**
> "HTTP methods define the type of action. GET is for fetching data, POST is for creating data, PUT is for updating data, and DELETE is for removing data."

**Q4. What are HTTP status codes?**
> "Status codes tell the client what happened with the request. 200 means success, 201 means created, 301 means redirect, 400 means bad request, 401 means unauthorized, 404 means not found, and 500 means internal server error."

**Q5. What is SSL/TLS?**
> "SSL and TLS are encryption protocols that secure data transmitted between client and server. When you see HTTPS and a lock icon in the browser, TLS is working in the background to encrypt all communication."

**Q6. Why is HTTPS important in system design?**
> "HTTPS protects user data from man in the middle attacks where someone intercepts communication between client and server. All production systems must use HTTPS especially for authentication, payments and sensitive data."

**Q7. What is the difference between HTTP/1.1 and HTTP/2?**
> "HTTP/1.1 sends one request at a time per connection causing a bottleneck. HTTP/2 allows multiple requests over a single connection simultaneously — this is called multiplexing. HTTP/2 is significantly faster and used by most modern websites."
