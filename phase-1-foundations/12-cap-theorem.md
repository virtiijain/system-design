# CAP Theorem

## Diagram
```
         CONSISTENCY
              △
             / \
            /   \
           / CP  \
          /       \
         ▽───────────▽
  PARTITION        AVAILABILITY
  TOLERANCE      AP

CP → consistent + partition tolerant
     example → banks, ATMs

AP → available + partition tolerant
     example → Netflix, Twitter
```

## Interview Questions

**Q1. What is CAP theorem?**
> "CAP theorem states that a distributed system can only guarantee two out of three — Consistency, Availability and Partition Tolerance. You cannot have all three at the same time."

**Q2. What is consistency in CAP?**
> "Consistency means every user sees the same data at the same time. If I update my profile, everyone should see the updated profile immediately."

**Q3. What is availability in CAP?**
> "Availability means the system always responds to requests. Even if some servers are down, it never returns an error — always gives back some response."

**Q4. What is partition tolerance?**
> "Partition tolerance means the system works even if network breaks between servers. In real world, network failures always happen — so partition tolerance is always required."

**Q5. Why can we only pick two out of three?**
> "Partition tolerance is mandatory in real world. So real choice is between consistency and availability. During network partition, either return correct data and risk being unavailable, or stay available and risk returning stale data."

**Q6. Give real world examples of CP and AP systems?**
> "CP systems — banks and payments. If servers cannot sync, system becomes unavailable rather than showing wrong balance. AP systems — Netflix and Twitter. They may show slightly stale data but never go down."
