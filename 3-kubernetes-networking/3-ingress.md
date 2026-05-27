## What is Ingress?

Ingress exposes HTTP/HTTPS routes into Kubernetes.

---

# Why Ingress?

Without ingress:

```text
Each service needs separate LoadBalancer
```

Expensive and inefficient.

---

# With Ingress

Single entry point handles routing.

Example:

```text
/api  -> backend-service
/auth -> auth-service
```

---

# Ingress Components

| Component | Purpose |
|---|---|
| Ingress Resource | Routing rules |
| Ingress Controller | Implements rules |

---

# Popular Ingress Controllers

| Controller | Description |
|---|---|
| NGINX Ingress | Most popular |
| Traefik | Kubernetes-native |
| HAProxy | High-performance |
| Istio Gateway | Service mesh gateway |

---

# Example Ingress YAML

```yaml
apiVersion: networking.k8s.io/v1
kind: Ingress
metadata:
  name: app-ingress

spec:
  rules:
    - host: myapp.com
      http:
        paths:
          - path: /
            pathType: Prefix
            backend:
              service:
                name: frontend-service
                port:
                  number: 80
```

---

# TLS with Ingress

Ingress can terminate TLS.

Example:

```yaml
tls:
  - hosts:
      - myapp.com
```

---

# Ingress Request Flow

```text
User
  ↓
Load Balancer
  ↓
Ingress Controller
  ↓
Service
  ↓
Pod
```

---
