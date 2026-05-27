## What is Circuit Breaker?

Circuit breaker prevents repeated failures from overwhelming systems.

---

# Real-World Analogy

Electrical circuit breaker:

```text
Too much current -> Breaker opens
```

Software circuit breaker:

```text
Too many failures -> Requests blocked
```

---

# Circuit Breaker States

| State | Description |
|---|---|
| Closed | Normal traffic |
| Open | Requests blocked |
| Half-Open | Testing recovery |

---

# Example Flow

```text
Backend failing repeatedly
        ↓
Circuit opens
        ↓
Traffic temporarily blocked
```

---

# Benefits

- Prevent cascading failures
- Faster recovery
- Protect downstream systems

---

# Used In

- Istio
- Envoy
- Resilience4j
- Hystrix

---