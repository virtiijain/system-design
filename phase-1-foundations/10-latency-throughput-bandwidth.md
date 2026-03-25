# Latency, Throughput, Bandwidth

## Diagram
```
BANDWIDTH = 100 Mbps (max capacity)
      │
      │ congestion, packet loss
      ▼
THROUGHPUT = 60 Mbps (actual)
      │
      │ distance, processing
      ▼
LATENCY = 20ms (delay per request)
```

## Interview Questions

**Q1. What is latency?**
> "Latency is the time taken for a request to travel from client to server and back. Measured in milliseconds. Lower latency means faster response and better user experience."

**Q2. What is throughput?**
> "Throughput is the actual amount of data successfully transferred per second. Always less than bandwidth due to network congestion and packet loss."

**Q3. What is bandwidth?**
> "Bandwidth is the maximum capacity of a network — the maximum data that can transfer per second. Like the width of a pipe — wider pipe means more data can flow."

**Q4. What is the difference between bandwidth and throughput?**
> "Bandwidth is theoretical maximum under perfect conditions. Throughput is actual real world measurement. Throughput is always lower than bandwidth due to congestion and overhead."

**Q5. How do you reduce latency in system design?**
> "Use CDN to serve content closer to users, cache frequently accessed data, reduce network hops, use faster databases and optimize code to process requests faster."

**Q6. Why does latency matter?**
> "Even 100ms extra latency can reduce conversions on an e-commerce site. In real time systems like stock trading or gaming, even 1ms matters. Reducing latency is a core goal of system design."
