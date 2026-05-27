## Why Services Exist

Pods are ephemeral.

Their IP addresses change frequently.

Services provide stable networking endpoints.

---

# Service Types

| Service Type | Purpose |
|---|---|
| ClusterIP | Internal communication |
| NodePort | External access via node |
| LoadBalancer | Cloud load balancer |
| ExternalName | External DNS mapping |

---

# ClusterIP

Default service type.

Accessible only inside cluster.

Example:

```text
frontend-pod
      ↓
payment-service
      ↓
backend-pods
```

---

# NodePort

Exposes service on node IP and port.

Example:

```text
NodeIP:30080
```

---

# LoadBalancer

Creates cloud load balancer automatically.

Supported in:

- AWS
- GCP
- Azure

---

# ExternalName

Maps Kubernetes service to external DNS.

Example:

```text
database.example.com
```

---

# Example Service YAML

```yaml
apiVersion: v1
kind: Service
metadata:
  name: backend-service

spec:
  selector:
    app: backend

  ports:
    - protocol: TCP
      port: 80
      targetPort: 8080

  type: ClusterIP
```

---
