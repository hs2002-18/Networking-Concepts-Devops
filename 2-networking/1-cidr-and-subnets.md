## What is CIDR?

CIDR (Classless Inter-Domain Routing) defines IP ranges.

Example:

```text
192.168.1.0/24
```

---

## Understanding CIDR

```text
/24 = 24 network bits
```

Available IP range:

```text
192.168.1.1 - 192.168.1.254
```

Total IPs:

```text
256
```

---

## Common CIDR Ranges

| CIDR | Total IPs |
|---|---|
| /32 | 1 |
| /30 | 4 |
| /24 | 256 |
| /16 | 65,536 |

---
## What is Subnetting?

Subnetting divides a large network into smaller networks.

Example:

```text
10.0.0.0/16
```

Split into:

```text
10.0.1.0/24
10.0.2.0/24
10.0.3.0/24
```

---

## Public vs Private Subnets

| Public Subnet | Private Subnet |
|---|---|
| Has internet access | No direct internet |
| Used for Load Balancers | Used for DB/App |
| Has public IPs | Uses private IPs |

---

## Why Subnetting Matters

- Better security
- Isolation
- Scalability
- Better IP management
- Reduced blast radius

---