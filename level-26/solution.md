# Bandit Level 26 → 27

## Commands

```bash
ls -la
./bandit27-do cat /etc/bandit_pass/bandit27
```

## Why this works

The setuid `bandit27-do` helper executes a supplied command with the privileges needed to read the next password file.
