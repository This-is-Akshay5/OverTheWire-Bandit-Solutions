# Bandit Level 16 → 17

## Commands

```bash
nmap -p 31000-32000 localhost
openssl s_client -connect localhost:31790 -quiet
```

Submit the current password to the correct TLS service.

## Why this works

`nmap` identifies the open ports. The relevant TLS service returns an OpenSSH private key after receiving the correct password.
