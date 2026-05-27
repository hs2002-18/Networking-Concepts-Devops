## What are Security Groups?

Security Groups are virtual firewalls for cloud resources.

They control:

- Inbound traffic
- Outbound traffic

---

## Example HTTPS Rule

| Type | Port | Source |
|---|---|---|
| HTTPS | 443 | 0.0.0.0/0 |

---

## Example Database Rule

Allow MySQL only from application servers.

| Port | Source |
|---|---|
| 3306 | App Security Group |

---

## Stateful Firewall

Security groups are stateful.

If inbound traffic allowed:

```text
Return traffic automatically allowed
```

---

## Security Group Best Practices

- Restrict SSH access
- Avoid open ports
- Use least privilege
- Separate app and DB security groups

---