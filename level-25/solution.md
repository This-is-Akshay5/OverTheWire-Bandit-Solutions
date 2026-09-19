# Bandit Level 25 → 26

## Commands

Copy and validate the provided key:

```cmd
scp -P 2220 bandit25@bandit.labs.overthewire.org:/home/bandit25/bandit26.sshkey D:\bandit26.sshkey
ssh-keygen -y -f D:\bandit26.sshkey
```

In a suitable terminal:

```bash
ssh -i ~/bandit26.sshkey bandit26@bandit.labs.overthewire.org -p 2220
```

Use the `more`/Vim escape:

```vim
v
:shell
```

Then:

```bash
cat /etc/bandit_pass/bandit27
```

## Why this works

The next account is forced through a small terminal pager. Opening Vim from `more` and spawning a shell escapes that restriction, allowing commands to run as the authenticated account.
