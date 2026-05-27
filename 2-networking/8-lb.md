## What is Load Balancing?

Load balancing distributes traffic across multiple servers.

---

## Benefits

- High availability
- Scalability
- Fault tolerance
- Better performance

---

## Example

```text
              Load Balancer
                    ↓
      -------------------------
      ↓           ↓           ↓
    App-1       App-2       App-3
```

---

## Layer 4 vs Layer 7

| Layer 4 | Layer 7 |
|---|---|
| TCP/UDP | HTTP/HTTPS |
| Faster | Smarter routing |
| Less context | Path-based routing |

---

## Common Algorithms

| Algorithm | Description |
|---|---|
| Round Robin | Sequential |
| Least Connections | Least traffic |
| IP Hash | Based on client IP |
| Weighted | Based on server capacity |

---

## Health Checks

Load balancer continuously checks:

```text
Is backend healthy?
```

Unhealthy servers removed automatically.

---

## Sticky Sessions

Ensures same client reaches same backend.

Useful for:

- Session-based apps
- Legacy applications

---