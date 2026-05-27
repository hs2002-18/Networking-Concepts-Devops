# 7. TLS/SSL

## What is TLS?

TLS (Transport Layer Security) encrypts communication between client and server.

HTTPS uses TLS.

SSL is older and mostly replaced by TLS.

---

## Goals of TLS

| Goal | Purpose |
|---|---|
| Encryption | Prevent data theft |
| Integrity | Prevent tampering |
| Authentication | Verify server identity |

---

## TLS Handshake Flow

```text
Client Hello
    ↓
Server Hello
    ↓
Certificate Exchange
    ↓
Key Exchange
    ↓
Encrypted Communication
```

---

## TLS Handshake Steps

### Step 1: Client Hello

Browser sends:

- Supported TLS versions
- Supported cipher suites

---

### Step 2: Server Hello

Server responds with:

- Selected TLS version
- Cipher suite
- SSL certificate

---

### Step 3: Certificate Validation

Browser validates:

- Certificate issuer
- Expiration date
- Domain match

---

### Step 4: Key Exchange

Encryption keys exchanged securely.

---

### Step 5: Secure Communication

All traffic becomes encrypted.

---

## TLS Versions

| Version | Status |
|---|---|
| SSL 2.0 | Obsolete |
| SSL 3.0 | Obsolete |
| TLS 1.0 | Deprecated |
| TLS 1.2 | Widely used |
| TLS 1.3 | Modern standard |

---

## SSL Termination

Reverse proxy or load balancer handles TLS.

Example:

```text
User HTTPS Request
      ↓
NGINX Terminates TLS
      ↓
Backend HTTP Traffic
```

---

## Useful Commands

### View Certificate

```bash
openssl s_client -connect google.com:443
```

### Test HTTPS

```bash
curl -v https://google.com
```

---

# Common DevOps Networking Commands

| Command | Purpose |
|---|---|
| curl | Test APIs |
| dig | DNS lookup |
| nslookup | DNS troubleshooting |
| netstat | View network connections |
| ss | Socket statistics |
| traceroute | View packet path |
| tcpdump | Packet capture |

---