## What is CNI?

CNI plugins provide networking for Kubernetes pods.

They are responsible for:

- Pod IP allocation
- Networking
- Routing
- Network policies

---

# Popular CNI Plugins

| CNI | Description |
|---|---|
| Calico | Networking + Policies |
| Flannel | Simple overlay network |
| Cilium | eBPF-based networking |
| Weave | Multi-host networking |

---

# CNI Flow

```text
Pod Created
      ↓
CNI Assigns IP
      ↓
Routes Configured
      ↓
Pod Connected to Network
```

---

# Calico

Popular for:

- Network policies
- Security
- Scalability

---

# Cilium

Uses eBPF.

Provides:

- High performance
- Deep observability
- Advanced security

---
