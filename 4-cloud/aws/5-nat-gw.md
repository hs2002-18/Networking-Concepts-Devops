## What is NAT Gateway?

Allows private resources to access internet securely.

---

# Why NAT Gateway is Needed

Private instances need internet access for:

- Package installation
- Docker pulls
- Security updates
- External APIs

Without exposing themselves publicly.

---

# NAT Flow

```text
Private EC2
     ↓
NAT Gateway
     ↓
Internet
```

---

# NAT Gateway Best Practices

- Place NAT in public subnet
- Use one NAT per AZ
- Avoid single point of failure

---

# NAT Gateway vs NAT Instance

| NAT Gateway | NAT Instance |
|---|---|
| Managed | Self-managed |
| Highly available | Manual scaling |
| Easier setup | More control |

---