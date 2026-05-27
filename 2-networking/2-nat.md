## What is NAT?

NAT allows private servers to access internet using a public IP.

---

## Why NAT is Needed

Private IPs are not routable on internet.

Private ranges:

```text
10.0.0.0/8
172.16.0.0/12
192.168.0.0/16
```

---

## NAT Flow

```text
Private Server
      ↓
NAT Gateway
      ↓
Internet
```

Internet sees only NAT public IP.

---

## NAT Gateway vs NAT Instance

| NAT Gateway | NAT Instance |
|---|---|
| Managed service | Self-managed |
| Highly available | Manual setup |
| Auto scaling | Manual scaling |

---

## DevOps Use Cases

Private servers use NAT to:

- Download packages
- Pull Docker images
- Access external APIs
- Install updates

Without exposing themselves publicly.

---