# Bandit Level 20 → 21

## Commands

Terminal 1:
```bash
nc -lvnp 12345
```

Terminal 2:
```bash
./suconnect 12345
```

Then enter the current password in the listener.

## Why this works

`suconnect` connects to a local listening port and validates the password sent over that connection.
