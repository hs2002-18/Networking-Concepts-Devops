## Core Networking Principle

Every pod gets:

- Its own IP address
- Direct communication capability

Pods should communicate without NAT.

---

# Kubernetes Networking Rules

| Rule | Description |
|---|---|
| Pod-to-Pod Communication | Allowed |
| Node-to-Pod Communication | Allowed |
| No NAT Between Pods | Required |

---

# Example

```text
Pod-A (10.244.1.5)
        ↓
Pod-B (10.244.2.8)
```

Pods communicate directly using IPs.

---

# Why Kubernetes Networking is Different

Traditional infrastructure:

```text
VM -> IP
```

Kubernetes:

```text
Every Pod -> Separate IP
```

This creates dynamic networking challenges.

---