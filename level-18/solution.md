# Bandit Level 18 → 19

## Commands

```cmd
ssh bandit18@bandit.labs.overthewire.org -p 2220 "cat readme"
```

## Why this works

The normal interactive shell immediately exits because of the level's shell configuration. Supplying a remote command runs `cat` directly before the shell terminates.
