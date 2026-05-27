## What is Rate Limiting?

Rate limiting restricts number of requests.

---

# Why Rate Limiting Matters

Protects systems from:

- Abuse
- Bots
- DDoS
- Overload

---

# Example

```text
100 requests per minute
```

---

# Common Algorithms

| Algorithm | Description |
|---|---|
| Token Bucket | Controlled bursts |
| Leaky Bucket | Constant rate |
| Fixed Window | Simple counter |
| Sliding Window | More accurate |

---

# Example API Response

```http
429 Too Many Requests
```

---

# Where Rate Limiting is Used

- APIs
- API gateways
- Load balancers
- Ingress controllers

---