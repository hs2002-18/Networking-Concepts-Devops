## What is an Internet Gateway?

Internet Gateway allows communication between:

```text
VPC <-> Internet
```

---

## Requirements for Internet Access

A subnet requires:

- Internet Gateway
- Public IP
- Route table entry

---

## Example

```text
0.0.0.0/0 -> Internet Gateway
```

---

## Common Use Cases

- Public websites
- APIs
- Bastion hosts
- Load balancers

---
