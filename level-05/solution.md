# Bandit Level 5 → 6

## Commands

```bash
cd ~/inhere
find . -type f -size 1033c ! -executable
cat ./maybehere07/.file2
```

## Why this works

`find` filters files by the required size and non-executable property, narrowing the search to the target file.
