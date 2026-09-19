# Bandit Level 12 → 13

## Commands

```bash
mktemp -d
cd /tmp/<temporary-directory>
cp ~/data.txt .
mv data.txt data.hex
xxd -r data.hex data
file data
```

Then repeatedly rename/decompress/extract according to the type reported by `file`, using `gzip -d`, `bzip2 -d`, and `tar -xf` until the final plaintext is reached.

## Why this works

The file is a hexadecimal dump containing several layers of compression and archiving. `xxd -r`, `file`, and the matching decompression/extraction tools peel off each layer.
