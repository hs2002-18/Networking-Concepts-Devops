
## What is a Reverse Proxy?

A reverse proxy sits between users and backend servers.

```text
Client -> Reverse Proxy -> Backend
```

---

## Benefits

| Feature | Benefit |
|---|---|
| SSL Termination | Centralized TLS |
| Security | Hide backend |
| Compression | Faster responses |
| Caching | Better performance |
| Routing | Traffic management |

---

## Popular Reverse Proxies

| Tool | Description |
|---|---|
| NGINX | Most popular |
| HAProxy | High performance |
| Envoy | Cloud-native proxy |
| Traefik | Kubernetes friendly |

---

## Example NGINX Config

```nginx
server {
    listen 80;

    location / {
        proxy_pass http://backend;
    }
}
```

---