## What is Load Balancer?

Distributes traffic across multiple targets.

---

# Types of AWS Load Balancers

| Type | Layer | Use Case |
|---|---|---|
| ALB | Layer 7 | HTTP/HTTPS |
| NLB | Layer 4 | TCP/UDP |
| GWLB | Layer 3/4 | Security appliances |

---

# Application Load Balancer (ALB)

Supports:

- Path-based routing
- Host-based routing
- TLS termination

---

# Example

```text
/api -> Backend Service
/auth -> Auth Service
```

---

# Network Load Balancer (NLB)

Used for:

- High performance
- TCP traffic
- Low latency

---

# Health Checks

Load balancer continuously checks:

```text
Is target healthy?
```

Unhealthy targets removed automatically.

---
