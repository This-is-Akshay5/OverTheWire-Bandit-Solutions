# Bandit Level 1 → 2

## Commands

```bash
cat ./-
```

## Why this works

The file is literally named `-`, which many commands interpret as standard input. `./-` explicitly identifies it as a filename.
