# Bandit Level 6 → 7

## Commands

```bash
find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
cat /var/lib/dpkg/info/bandit7.password
```

## Why this works

The challenge specifies the file's owner, group, size, and location somewhere under `/`. `find` searches those attributes while `2>/dev/null` hides permission errors.
