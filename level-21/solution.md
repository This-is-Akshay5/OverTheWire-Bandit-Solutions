# Bandit Level 21 → 22

## Commands

```bash
ls -la /etc/cron.d/
cat /etc/cron.d/cronjob_bandit22
cat /usr/bin/cronjob_bandit22.sh
cat /tmp/<path-shown-by-the-script>
```

## Why this works

A cron job periodically copies the next level's password into a predictable temporary file. Reading that generated file reveals the password.
