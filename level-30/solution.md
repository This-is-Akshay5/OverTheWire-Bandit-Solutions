# Bandit Level 30 → 31

## Commands

```cmd
mkdir D:\bandit30
cd /d D:\bandit30
git clone ssh://bandit30-git@bandit.labs.overthewire.org:2220/home/bandit30-git/repo
cd repo
type README.md
git tag
git show secret
```

## Why this works

The repository README is intentionally empty, but a Git tag named `secret` contains the hidden credential.
