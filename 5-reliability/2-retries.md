## What are Retries?

Retries automatically resend failed requests.

---

# Why Retries Matter

Distributed systems fail temporarily.

Example:

- Network glitch
- DNS delay
- Temporary overload

Retries help recover automatically.

---

# Example Retry Flow

```text
Request Failed
      ↓
Retry
      ↓
Success
```

---

# Retry Example

```yaml
retries: 3
```

---

# Retry Risks

Too many retries can cause:

- Traffic spikes
- Cascading failures
- Backend overload

---

# Best Practices

- Use limited retries
- Combine with backoff
- Avoid infinite retries

---

# Retryable Errors

| Error | Retry? |
|---|---|
| Timeout | Yes |
| 503 Service Unavailable | Yes |
| DNS temporary failure | Yes |
| 401 Unauthorized | No |
| 404 Not Found | Usually No |

---
