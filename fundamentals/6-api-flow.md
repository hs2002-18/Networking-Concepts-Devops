## What is an API?

API (Application Programming Interface) allows applications to communicate.

Example:

```text
Frontend -> Backend API -> Database
```

---

## Typical API Flow

```text
Client
  ↓
DNS
  ↓
Load Balancer
  ↓
API Gateway
  ↓
Authentication
  ↓
Application Service
  ↓
Database
```

---

## API Authentication Methods

| Method | Description |
|---|---|
| API Key | Simple token |
| JWT | Stateless authentication |
| OAuth | Third-party authentication |
| Session Cookie | Traditional login |

---

## API Gateway Features

- Authentication
- Logging
- Monitoring
- Routing
- Rate limiting

Examples:

- Kong
- AWS API Gateway
- Apigee
- NGINX

---

## Common API Problems

| Problem | Cause |
|---|---|
| Timeout | Slow backend |
| 401 Unauthorized | Invalid token |
| High latency | DB/API issue |
| 429 Too Many Requests | Rate limit exceeded |

---