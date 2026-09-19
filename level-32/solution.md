# Bandit Level 32 → 33

## Commands

```cmd
ssh bandit32@bandit.labs.overthewire.org -p 2220
```

Inside the uppercase shell:

```bash
$0
whoami
cat /etc/bandit_pass/bandit33
```

## Why this works

The uppercase shell transforms normal commands, but `$0` invokes the shell itself and escapes the restricted command behavior. A normal shell then allows the password file to be read.
