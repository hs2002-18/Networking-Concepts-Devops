## What is a Route Table?

Defines where traffic should go.

---

# Example Route Table

| Destination | Target |
|---|---|
| 10.0.0.0/16 | Local |
| 0.0.0.0/0 | Internet Gateway |

---

# Public Route Table

```text
0.0.0.0/0 -> Internet Gateway
```

---

# Private Route Table

```text
0.0.0.0/0 -> NAT Gateway
```

---

# Why Route Tables Matter

Controls:

- Internet access
- VPN traffic
- Peering traffic
- Hybrid networking

---