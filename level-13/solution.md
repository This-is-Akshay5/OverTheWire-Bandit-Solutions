# Bandit Level 13 → 14

## Commands

```cmd
scp -P 2220 bandit13@bandit.labs.overthewire.org:sshkey.private C:\Users\admin\sshkey.private
ssh -i C:\Users\admin\sshkey.private bandit14@bandit.labs.overthewire.org -p 2220
```

Then:

```bash
cat /etc/bandit_pass/bandit14
```

## Why this works

The level provides a private SSH key for the next account. `scp` copies it locally and `ssh -i` authenticates with that key.
