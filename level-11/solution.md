# Bandit Level 11 → 12

## Commands

```bash
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

## Why this works

The text uses ROT13. `tr` maps each alphabetic character to its ROT13 counterpart.
