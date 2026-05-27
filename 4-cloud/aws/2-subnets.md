## What is a Subnet?

Subnet divides VPC into smaller networks.

---

# Example

VPC:

```text
10.0.0.0/16
```

Subnets:

```text
10.0.1.0/24
10.0.2.0/24
10.0.3.0/24
```

---

# Public Subnet

Has:

- Internet Gateway route
- Public IP support

Usually contains:

- Load balancers
- Bastion hosts

---

# Private Subnet

No direct internet access.

Usually contains:

- Application servers
- Databases
- EKS worker nodes

---

# High Availability Best Practice

Use multiple AZs.

Example:

```text
Public Subnet AZ-A
Public Subnet AZ-B

Private Subnet AZ-A
Private Subnet AZ-B
```

---