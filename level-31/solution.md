# Bandit Level 31 → 32

## Commands

```cmd
mkdir D:\bandit31
cd /d D:\bandit31
git clone ssh://bandit31-git@bandit.labs.overthewire.org:2220/home/bandit31-git/repo
cd repo
```

Create the required file and force-add it because `.gitignore` excludes it:

```cmd
powershell -Command "[IO.File]::WriteAllText('key.txt', 'May I come in?' + [char]10, [Text.UTF8Encoding]::new($false))"
git add -f key.txt
git commit -m "add key"
git push
```

If Windows line-ending conversion causes validation to fail, amend the commit after writing the file with the PowerShell command above:

```cmd
git add -f key.txt
git commit --amend --no-edit
git push origin master
```

## Why this works

The remote pre-receive hook validates a specific file, content, and branch. `git add -f` bypasses the local ignore rule, while the explicit LF write avoids Windows CRLF line endings.
