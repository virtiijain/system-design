# Client Server Model

**Q1. What is the client server model?**
> "Client server model is an architecture where the client sends a request and the server processes it and sends back a response. The client is usually a browser or mobile app, and the server handles business logic and data."

**Q2. What is the difference between client and server?**
> "A client initiates communication — it sends requests. A server waits for requests, processes them, and returns responses. A client is usually user-facing like a browser, while a server runs in the background handling logic and data."

**Q3. What is an API?**
> "API stands for Application Programming Interface. It is the contract between client and server — it defines what requests can be made, in what format, and what response will come back."

**Q4. Can a server also be a client?**
> "Yes, absolutely. In microservices architecture, servers frequently call other servers. So a server handling your request might itself act as a client and call another service — like a payment service or notification service."

**Q5. What happens if the server goes down?**
> "If the server goes down, clients cannot get responses — the app becomes unavailable. This is why in system design we use multiple servers, load balancers, and failover mechanisms to ensure no single point of failure."