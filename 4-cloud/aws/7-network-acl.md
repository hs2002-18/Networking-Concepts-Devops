## What are NACLs?

Subnet-level firewalls.

---

# Security Group vs NACL

| Security Group | NACL |
|---|---|
| Stateful | Stateless |
| Resource-level | Subnet-level |
| Allow only | Allow + Deny |

---

# NACL Example

| Rule | Action |
|---|---|
| Allow 80 | ALLOW |
| Deny IP | DENY |

---

# When NACLs are Useful

- Blocking malicious IPs
- Extra security layer
- Compliance requirements

---