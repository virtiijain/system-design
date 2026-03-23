# TCP / IP

## Diagram
```
TCP 3-WAY HANDSHAKE

CLIENT                    SERVER
  │                          │
  │───── SYN ───────────────►│  "can we connect?"
  │◄──────────── SYN-ACK ────│  "yes, ready!"
  │───── ACK ───────────────►│  "great, let's go!"
  │                          │
  │═══════ DATA FLOWS ══════►│
  │◄══════════════════ ACK ══│  "received!"

─────────────────────────────────────

DATA PACKETS

BIG DATA
    │
    ▼
┌────────┐ ┌────────┐ ┌────────┐
│Packet 1│ │Packet 2│ │Packet 3│  → sent separately
└────────┘ └────────┘ └────────┘
              │
              ▼
       RECEIVER joins all
       packets in order
              │
              ▼
         FULL DATA ✓

─────────────────────────────────────

TCP vs UDP

TCP → reliable, ordered, slower  → web, email, files
UDP → fast, no guarantee         → video calls, gaming
```

## 🎯 Interview Questions

**Q1. What is TCP/IP?**
> "TCP/IP is the foundational communication protocol of the internet. IP handles addressing — where to send the data. TCP handles reliability — ensures data arrives completely and in order."

**Q2. What is the TCP 3-way handshake?**
> "Before sending data, TCP establishes connection using 3-way handshake. Client sends SYN — I want to connect. Server replies SYN-ACK — I am ready. Client sends ACK — let's go. Only then data transfer begins."

**Q3. What are packets?**
> "Data is broken into small chunks called packets. Each packet travels independently and may take different routes. TCP reassembles them in correct order at the destination."

**Q4. What is the difference between TCP and UDP?**
> "TCP is reliable — guarantees delivery, order and error checking but slower. UDP is faster but unreliable — sends data without confirming delivery. TCP is used for web and file transfers. UDP is used for video calls and gaming where speed matters more than perfection."

**Q5. Why is TCP/IP important in system design?**
> "TCP/IP is the backbone of all internet communication. Understanding it helps design systems that handle network failures, retries and timeouts. Knowing TCP has overhead helps decide when to use UDP for latency sensitive apps like video streaming."
