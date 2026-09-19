# Bandit Level 19 → 20

## Commands

```bash
ls -la
./bandit20-do
./bandit20-do cat /etc/bandit_pass/bandit20
```

## Why this works

`bandit20-do` is a setuid helper that executes a command with the required privileges. Reading the next password file therefore succeeds.
