## What is HTTP?

HTTP (HyperText Transfer Protocol) is used for communication between client and server.

HTTPS = HTTP + TLS encryption.

---

# Complete HTTP Lifecycle

Example:

```text
https://myapp.com/login
```

---

## Step 1: DNS Resolution

Domain resolves into IP address.

---

## Step 2: TCP Handshake

TCP connection established.

---

## Step 3: TLS Handshake

Secure encrypted channel created.

---

## Step 4: HTTP Request Sent

Example:

```http
GET /login HTTP/1.1
Host: myapp.com
```

---

## Step 5: Reverse Proxy

Traffic usually reaches:

- NGINX
- HAProxy
- Envoy

---

## Step 6: Load Balancer

Traffic distributed across backend servers.

---

## Step 7: Application Processing

Backend:

- Validates request
- Accesses database
- Calls APIs

---

## Step 8: Response Returned

```http
HTTP/1.1 200 OK
```

Returned to browser.

---

## Common HTTP Methods

| Method | Purpose |
|---|---|
| GET | Retrieve data |
| POST | Create resource |
| PUT | Update resource |
| PATCH | Partial update |
| DELETE | Remove resource |

---

## Common HTTP Status Codes

| Code | Meaning |
|---|---|
| 200 | Success |
| 201 | Created |
| 400 | Bad Request |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |
| 500 | Internal Error |
| 502 | Bad Gateway |
| 504 | Gateway Timeout |

---