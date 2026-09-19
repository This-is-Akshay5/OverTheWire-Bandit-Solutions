# Bandit Level 9 → 10

## Commands

```bash
strings data.txt | grep "==="
```

## Why this works

The target is hidden among binary/non-printable data. `strings` extracts readable text and `grep` finds the marker used around the password.
