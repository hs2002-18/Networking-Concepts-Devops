## What is Internet Gateway?

Allows communication between:

```text
VPC <-> Internet
```

---

# Requirements for Public Access

A subnet requires:

- Internet Gateway
- Public IP
- Route table entry

---

# Example

```text
0.0.0.0/0 -> IGW
```

---

# Common Use Cases

- Public websites
- APIs
- Bastion hosts
- Public load balancers

---
