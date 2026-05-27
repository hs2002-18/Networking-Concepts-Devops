## What is a Timeout?

A timeout defines:

```text
How long a service waits before giving up
```

---

# Why Timeouts Matter

Without timeouts:

- Requests can hang forever
- Threads can get blocked
- Systems can become overloaded

---

# Example

```text
Frontend
   ↓
Backend API
   ↓
Database
```

If database becomes slow:

```text
Frontend waits forever
```

Timeout prevents this.

---

# Types of Timeouts

| Timeout | Purpose |
|---|---|
| Connection Timeout | Wait for connection |
| Read Timeout | Wait for response |
| Idle Timeout | Inactive connection timeout |
| Request Timeout | Total request duration |

---

# Example Timeout

```yaml
timeout: 5s
```

---

# Common Timeout Problems

| Problem | Cause |
|---|---|
| Too low | False failures |
| Too high | Resource exhaustion |
| No timeout | Hanging requests |

---

# DevOps Relevance

Timeouts are configured in:

- NGINX
- HAProxy
- Kubernetes Ingress
- APIs
- Databases
- Service Mesh

---
