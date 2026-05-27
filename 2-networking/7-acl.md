## What are Network ACLs?

NACLs are subnet-level firewalls.

---

## Security Group vs NACL

| Security Group | NACL |
|---|---|
| Stateful | Stateless |
| Instance-level | Subnet-level |
| Allow only | Allow + Deny |

---

## Example NACL Rule

| Rule | Action |
|---|---|
| Allow Port 80 | ALLOW |
| Deny Specific IP | DENY |

---

## Why NACLs Matter

Useful for:

- Extra subnet security
- Blocking malicious IPs
- Compliance requirements

---