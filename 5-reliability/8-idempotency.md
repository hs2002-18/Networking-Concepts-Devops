
## What is Idempotency?

Repeated requests produce same result.

---

# Example

Payment API:

```text
POST /payment
```

Should not charge twice if retried.

---

# Why Important?

Retries can duplicate requests.

Idempotency prevents:

- Double payments
- Duplicate orders
- Duplicate processing

---

# Common Solutions

- Idempotency keys
- Request tracking
- Transaction IDs

---
