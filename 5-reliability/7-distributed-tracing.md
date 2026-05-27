## What is Distributed Tracing?

Tracing tracks request flow across services.

---

# Why Tracing Matters

Microservices are distributed.

Single request may touch:

```text
Frontend
   ↓
API Gateway
   ↓
Auth Service
   ↓
Payment Service
   ↓
Database
```

Tracing helps identify bottlenecks.

---

# Trace Components

| Component | Description |
|---|---|
| Trace | Entire request |
| Span | Single operation |
| Trace ID | Unique request ID |

---

# Popular Tracing Tools

- Jaeger
- Zipkin
- OpenTelemetry

---

# Example Problem Solved by Tracing

```text
Why is checkout API slow?
```

Tracing shows:

```text
Database query taking 4 seconds
```

---