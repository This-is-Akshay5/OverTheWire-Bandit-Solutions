# Bandit Level 15 → 16

## Commands

```bash
openssl s_client -connect localhost:30001
```

Enter the current password.

## Why this works

Port 30001 expects a TLS connection. `openssl s_client` establishes TLS and lets you send the password to the service.
