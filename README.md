# mingw64-packages

```bash
makepkg-mingw -sciCf --noconfirm
```

## download depends

```bash
for p in `curl -sL https://api.github.com/repos/dragonflylee/mingw-packages/releases/tags/MINGW64 | grep browser_download_url | cut -d\" -f4`; do curl -sLO $p; done
```