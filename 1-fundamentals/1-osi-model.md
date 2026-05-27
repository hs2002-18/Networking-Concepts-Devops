# 1. OSI Model

## What is the OSI Model?

The OSI (Open Systems Interconnection) model is a conceptual framework used to understand how systems communicate over a network.

It divides networking into 7 layers.

Each layer performs a specific responsibility.

---

## OSI Layers

| Layer | Name | Purpose | Examples |
|---|---|---|---|
| 7 | Application | User-facing protocols | HTTP, DNS |
| 6 | Presentation | Encryption and formatting | TLS/SSL |
| 5 | Session | Session management | APIs |
| 4 | Transport | Reliable communication | TCP, UDP |
| 3 | Network | Routing | IP |
| 2 | Data Link | MAC communication | Ethernet |
| 1 | Physical | Hardware transmission | Cables |

---

## Real Example

Opening:

```text
https://google.com
```

Flow:

| Layer | Action |
|---|---|
| Application | Browser sends HTTP request |
| Presentation | TLS encrypts traffic |
| Session | Session maintained |
| Transport | TCP ensures delivery |
| Network | IP routes packets |
| Data Link | Ethernet/WiFi sends frames |
| Physical | Electrical signals transmitted |

---

## Why OSI Matters in DevOps

| Problem | Layer |
|---|---|
| DNS issue | Layer 7 |
| TLS issue | Layer 6 |
| TCP timeout | Layer 4 |
| Routing issue | Layer 3 |
