# Bandit Level 28 → 29

## Commands

```cmd
mkdir D:\bandit28
cd /d D:\bandit28
git clone ssh://bandit28-git@bandit.labs.overthewire.org:2220/home/bandit28-git/repo
cd repo
type README.md
git log --oneline
git log -p
```

## Why this works

The current README has the password redacted, but Git history contains an earlier commit where the real value was present. `git log -p` exposes that historical change.
