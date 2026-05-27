## What is Kubernetes DNS?

Kubernetes uses CoreDNS for internal DNS resolution.

---

# Why DNS is Important

Services dynamically discover each other.

---

# Example DNS Name

```text
payment-service.default.svc.cluster.local
```

---

# DNS Flow

```text
Pod
  ↓
CoreDNS
  ↓
Service IP Returned
```

---

# Common DNS Problems

| Problem | Cause |
|---|---|
| DNS timeout | CoreDNS issue |
| Service unreachable | Wrong service name |
| Slow DNS | Network latency |

---

# Debug DNS

```bash
kubectl exec -it pod-name -- nslookup kubernetes.default
```

---