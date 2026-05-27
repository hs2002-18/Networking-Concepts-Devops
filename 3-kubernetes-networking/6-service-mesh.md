## What is Service Mesh?

Service mesh manages service-to-service communication.

---

# Problems Solved by Service Mesh

- Traffic management
- Retries
- Observability
- mTLS
- Circuit breaking

---

# Popular Service Meshes

| Service Mesh | Description |
|---|---|
| Istio | Most popular |
| Linkerd | Lightweight |
| Consul | HashiCorp ecosystem |

---

# Service Mesh Architecture

```text
App Container
      ↓
Sidecar Proxy
      ↓
Network
```

Usually uses Envoy proxy sidecars.

---

# Features

| Feature | Purpose |
|---|---|
| mTLS | Secure communication |
| Retries | Reliability |
| Tracing | Observability |
| Traffic Splitting | Canary deployments |

---

# Kubernetes Networking Debugging

## Check Pods

```bash
kubectl get pods -o wide
```

---

## Check Services

```bash
kubectl get svc
```

---

## Check Ingress

```bash
kubectl get ingress
```

---

## Test Connectivity

```bash
kubectl exec -it pod-name -- curl service-name
```

---

## Debug DNS

```bash
kubectl exec -it pod-name -- nslookup kubernetes.default
```

---

# Common Kubernetes Networking Problems

| Problem | Cause |
|---|---|
| Service unreachable | Wrong selector |
| DNS failure | CoreDNS issue |
| Pod communication failure | CNI issue |
| Ingress not working | Controller issue |
| Timeout | Network policy/firewall |

---
