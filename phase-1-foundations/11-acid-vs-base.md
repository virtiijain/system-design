# ACID vs BASE

## Diagram
```
ACID (SQL)
┌─────────────────────────────┐
│ TRANSACTION                 │
│ step 1 ✓                    │
│ step 2 ✓                    │
│ step 3 ✗ → ROLLBACK ALL     │
│ all or nothing              │
└─────────────────────────────┘

BASE (NoSQL)
┌─────────────────────────────┐
│ REQUEST                     │
│ → always responds ✓         │
│ → data may be slightly old  │
│ → will sync eventually ✓    │
└─────────────────────────────┘
```

## Interview Questions

**Q1. What is ACID?**
> "ACID stands for Atomicity, Consistency, Isolation and Durability. These properties guarantee reliable transaction processing in relational databases. ACID ensures data is always correct and never lost."

**Q2. What is atomicity?**
> "Atomicity means a transaction is all or nothing. If you transfer money — debit and credit both happen, or neither happens. If anything fails midway, everything is rolled back."

**Q3. What is isolation?**
> "Isolation means concurrent transactions do not interfere with each other. Two people booking the last seat at the same time — isolation ensures only one succeeds."

**Q4. What is BASE?**
> "BASE stands for Basically Available, Soft state and Eventually Consistent. Used in NoSQL databases. BASE prioritizes availability and performance over strict consistency."

**Q5. What is eventual consistency?**
> "Eventual consistency means data will become consistent across all servers, but not immediately. When you post on Instagram, followers in different regions may see it at slightly different times — but eventually everyone sees it."

**Q6. When to use ACID vs BASE?**
> "Use ACID when data correctness is critical — banking, payments, order management. Use BASE when availability and scale matter more — social media feeds, product catalogues, recommendation systems."

**Q7. What is the difference between ACID and BASE?**
> "ACID is strict and consistent — every transaction is perfect but slower. BASE is flexible and available — faster and more scalable but data may be temporarily inconsistent. ACID is for SQL, BASE is for NoSQL."
