## What is DNS?

DNS converts domain names into IP addresses.

Example:

```text
google.com -> 142.250.x.x
```

Humans remember names.

Computers communicate using IP addresses.

---

## DNS Resolution Flow

When opening:

```text
https://myapp.com
```

Flow:

```text
Browser
   ↓
Local Cache
   ↓
OS Resolver
   ↓
Recursive Resolver
   ↓
Root DNS Server
   ↓
TLD Server (.com)
   ↓
Authoritative Nameserver
   ↓
IP Address Returned
```

---
## DNS Record Types

| Record | Purpose |
|---|---|
| A | IPv4 mapping |
| AAAA | IPv6 mapping |
| CNAME | Alias |
| MX | Mail server |
| TXT | Verification |
| NS | Nameserver |

---

## TTL (Time To Live)

TTL defines how long DNS records stay cached.

Lower TTL:

- Faster updates
- More DNS requests

Higher TTL:

- Better performance
- Slower propagation

---

## Kubernetes DNS Example

```text
payment-service.default.svc.cluster.local
```

CoreDNS handles DNS in Kubernetes.

---

## DNS Commands

```bash
nslookup google.com

dig google.com

host google.com
```

---