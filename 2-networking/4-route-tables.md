## What is a Route Table?

Route tables define where network traffic should go.

---

## Example Route Table

| Destination | Target |
|---|---|
| 10.0.0.0/16 | Local |
| 0.0.0.0/0 | Internet Gateway |

---

## Public Route Table

Contains route to:

```text
0.0.0.0/0 -> Internet Gateway
```

Allows internet access.

---

## Private Route Table

Uses NAT Gateway:

```text
0.0.0.0/0 -> NAT Gateway
```

---

## Why Route Tables Matter

They control:

- Internet access
- Internal routing
- Hybrid networking
- VPN traffic

---