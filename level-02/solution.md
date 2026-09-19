# Bandit Level 2 → 3

## Commands

```bash
cat "./--spaces in this filename--"
```

## Why this works

The filename contains spaces and begins with hyphens. Quoting the complete path prevents the shell and `cat` from misinterpreting it.
