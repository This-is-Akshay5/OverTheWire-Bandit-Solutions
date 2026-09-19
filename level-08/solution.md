# Bandit Level 8 → 9

## Commands

```bash
sort data.txt | uniq -u
```

## Why this works

The password is the only line that occurs once. `sort` groups identical lines and `uniq -u` prints only unique entries.
