## What are Network Policies?

Network policies control pod-to-pod communication.

Acts like Kubernetes firewall.

---

# Why Network Policies Matter

By default:

```text
All pods can communicate
```

Network policies restrict communication.

---

# Example

Allow only frontend pods to access backend.

Block everything else.

---

# Example Network Policy

```yaml
apiVersion: networking.k8s.io/v1
kind: NetworkPolicy

metadata:
  name: backend-policy

spec:
  podSelector:
    matchLabels:
      app: backend

  policyTypes:
    - Ingress
```

---

# Benefits

- Security isolation
- Zero-trust networking
- Microservice protection

---
