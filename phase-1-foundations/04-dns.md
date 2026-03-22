# DNS (Domain Name System)

## Diagram
```
  you type google.com
        │
        ▼
  browser cache ── found? → done ✓
        │ not found
        ▼
  ISP DNS resolver
        │
        ▼
  root nameserver → "go to .com"
        │
        ▼
  .com nameserver → "go to google"
        │
        ▼
  google authoritative nameserver
        │
        ▼
  IP = 142.250.77.46 → browser connects ✓
```

## Interview Questions

**Q1. What is DNS?**
> "DNS stands for Domain Name System. It translates domain names like google.com into IP addresses so browsers can find the right server. Like a phonebook — name goes in, number comes out."

**Q2. How does DNS resolution work?**
> "Browser checks local cache first. If not found, queries ISP's DNS resolver. Resolver goes to root nameserver → TLD nameserver → authoritative nameserver which returns the actual IP. Browser then connects to that IP."

**Q3. What is TTL?**
> "TTL is Time To Live — how long a DNS record stays cached. Low TTL means faster updates but more queries. High TTL means fewer queries but slower propagation when IP changes."

**Q4. What is DNS caching?**
> "DNS caching saves the resolved IP locally so future requests skip the full lookup. Happens at browser, OS, router and ISP level — reduces latency significantly."

**Q5. Why is DNS important in system design?**
> "DNS is the entry point of every request. It can be used for load balancing by returning different IPs for the same domain. DNS latency directly impacts page load — so caching and TTL management are critical."

**Q6. What is the difference between authoritative and recursive DNS?**
> "Recursive resolver does the searching — queries multiple servers on your behalf. Authoritative server is the final source of truth — holds actual DNS records and returns IP directly."
