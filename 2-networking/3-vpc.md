## What is VPC?

A VPC is a logically isolated network inside cloud.

Think of it as:

```text
Your private datacenter in cloud
```

---

## VPC Components

| Component | Purpose |
|---|---|
| Subnet | Divide network |
| Route Table | Routing rules |
| Internet Gateway | Internet access |
| NAT Gateway | Outbound internet |
| Security Group | Firewall |
| NACL | Subnet firewall |

---

## Typical VPC Architecture

```text
Internet
   ↓
Load Balancer
   ↓
Public Subnet
   ↓
Private App Servers
   ↓
Database Subnet
```

---

## Public Subnet

Usually contains:

- Load balancers
- Bastion hosts
- Public-facing services

---

## Private Subnet

Usually contains:

- Application servers
- Databases
- Internal services

---