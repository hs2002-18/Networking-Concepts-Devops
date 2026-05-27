## What is VPN?

VPN securely connects networks over internet.

Example:

```text
Office Network <-> Cloud VPC
```

---

## VPN Benefits

- Secure communication
- Encrypted traffic
- Hybrid cloud connectivity

---

## VPC Peering

VPC peering connects two VPCs privately.

Traffic stays inside cloud network.

---

## Peering Example

```text
VPC-A <-> VPC-B
```

---

## Use Cases

- Multi-region applications
- Shared services
- Hybrid infrastructure

---

# Common Networking Commands

## Check Routes

```bash
ip route
```

---

## Check Connectivity

```bash
ping google.com
```

---

## DNS Lookup

```bash
dig google.com
```

---

## Check Open Ports

```bash
ss -tulnp
```

---

## Trace Packet Path

```bash
traceroute google.com
```

---

# Common Networking Problems

| Problem | Cause |
|---|---|
| High latency | Congestion |
| Packet loss | Network failure |
| Connection timeout | Firewall/routing |
| DNS failure | Resolver issue |
| TLS failure | Certificate issue |

---
