## What is Backoff?

Backoff delays retries gradually.

---

# Why Backoff Matters

Without backoff:

```text
Retries happen instantly
```

Can overload failing service.

---

# Exponential Backoff

Example:

```text
1s
2s
4s
8s
```

---

# Benefits

- Reduced traffic spikes
- Better recovery
- Improved stability

---

# Kubernetes Reliability Concepts

## Pod Restart Policies

Kubernetes automatically restarts failed pods.

---

# Auto Scaling

Automatically increases pods during high traffic.

---

# Self-Healing

Failed pods replaced automatically.

---

# Rolling Updates

Deployments updated gradually without downtime.

---

# Common Reliability Problems

| Problem | Cause |
|---|---|
| Cascading failures | Dependency overload |
| Retry storms | Excessive retries |
| High latency | Slow backend |
| Traffic spikes | No rate limiting |
| Resource exhaustion | Missing limits |

---

# DevOps Relevance

Reliability concepts are critical for:

- Production systems
- Kubernetes
- APIs
- Cloud-native apps
- Microservices
- High availability systems

---