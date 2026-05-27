## What is a VPC?

A VPC is a logically isolated network in AWS.

Think of it as:

```text
Your private datacenter inside AWS
```

---

# Example VPC

```text
10.0.0.0/16
```

---

# Why VPC is Important

VPC provides:

- Isolation
- Security
- Custom networking
- Routing control

---

# VPC Components

| Component | Purpose |
|---|---|
| Subnets | Divide network |
| Route Tables | Define routing |
| Internet Gateway | Internet access |
| NAT Gateway | Outbound internet |
| Security Groups | Firewall |
| NACLs | Subnet firewall |

---

# Typical AWS Architecture

```text
Internet
   ↓
Application Load Balancer
   ↓
Public Subnet
   ↓
Private App Servers
   ↓
Private Database
```

---
