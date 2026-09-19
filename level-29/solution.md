# Bandit Level 29 → 30

## Commands

```cmd
mkdir D:\bandit29
cd /d D:\bandit29
git clone ssh://bandit29-git@bandit.labs.overthewire.org:2220/home/bandit29-git/repo
cd repo
git branch -a
git checkout dev
type README.md
```

If necessary:

```cmd
git checkout sploits-dev
type README.md
```

## Why this works

The master branch does not contain the password. Git's remote branches contain additional development data, so checking them reveals the credential.
