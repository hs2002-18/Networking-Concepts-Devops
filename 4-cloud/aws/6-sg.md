## What are Security Groups?

Virtual firewalls attached to AWS resources.

---

# Security Group Characteristics

- Stateful
- Allow rules only
- Resource-level firewall

---

# Example Rules

## HTTPS Access

| Type | Port | Source |
|---|---|---|
| HTTPS | 443 | 0.0.0.0/0 |

---

## SSH Access

| Type | Port | Source |
|---|---|---|
| SSH | 22 | Your IP |

---

# Database Rule Example

Allow MySQL only from app servers.

| Port | Source |
|---|---|
| 3306 | App Security Group |

---

# Security Group Best Practices

- Restrict SSH access
- Never open DB publicly
- Use least privilege
- Separate app and DB SGs

---