## What are Health Checks?

Health checks determine whether service is healthy.

---

# Why Health Checks Matter

Unhealthy services should not receive traffic.

---

# Types of Health Checks

| Type | Purpose |
|---|---|
| Liveness Probe | Is app alive? |
| Readiness Probe | Ready for traffic? |
| Startup Probe | Slow startup apps |

---

# Kubernetes Example

```yaml
livenessProbe:
  httpGet:
    path: /health
    port: 8080
```

---

# Example Health Endpoint

```text
/health
```

Returns:

```json
{
  "status": "healthy"
}
```

---

# Common Problems

| Problem | Cause |
|---|---|
| False failures | Aggressive checks |
| No health checks | Traffic sent to bad pods |
| Slow checks | Increased latency |

---