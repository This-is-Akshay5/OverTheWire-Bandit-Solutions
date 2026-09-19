# Bandit Level 22 → 23

## Commands

```bash
cat /etc/cron.d/cronjob_bandit23
cat /usr/bin/cronjob_bandit23.sh
cat /tmp/$(echo I am user bandit23 | md5sum | cut -d ' ' -f 1)
```

## Why this works

The cron script hashes the string `I am user bandit23` to construct the output filename. Reproducing that calculation locates the generated password file.
