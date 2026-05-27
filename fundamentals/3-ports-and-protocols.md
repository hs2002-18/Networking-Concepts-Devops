## What is a Port?

A port identifies a specific service or application on a machine.

Example:

```text
IP Address -> Machine
Port -> Application
```

---

## Port Ranges

| Range | Purpose |
|---|---|
| 0-1023 | Well-known ports |
| 1024-49151 | Registered ports |
| 49152-65535 | Dynamic/private ports |

---

## Common Ports

| Service | Port |
|---|---|
| HTTP | 80 |
| HTTPS | 443 |
| SSH | 22 |
| DNS | 53 |
| MySQL | 3306 |
| PostgreSQL | 5432 |
| Kubernetes API | 6443 |
| Grafana | 3000 |
| Prometheus | 9090 |

---

## Common Protocols

| Protocol | Purpose |
|---|---|
| HTTP | Web communication |
| HTTPS | Secure web traffic |
| DNS | Domain resolution |
| SSH | Secure remote access |
| FTP | File transfer |

---

## Useful Commands

### Check Open Ports

```bash
netstat -tulnp

ss -tulnp
```

### Test HTTP

```bash
curl http://example.com
```

---