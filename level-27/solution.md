# Bandit Level 27 → 28

## Commands

```cmd
mkdir D:\bandit27
cd /d D:\bandit27
git clone ssh://bandit27-git@bandit.labs.overthewire.org:2220/home/bandit27-git/repo
cd repo
dir
type README
```

## Why this works

The challenge explicitly places the repository on a Git SSH endpoint. Cloning it locally and reading its README reveals the next credential.
