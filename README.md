AnimeXD - Auto Download Anime


# Guide to xdcc install

## Step 1: Download plugins

[Termux](https://www.f-droid.org/packages/com.termux/)

[Termux:Tasker](https://www.f-droid.org/packages/com.termux.tasker/)

## Step 2: Paste these into Termux

after install (hit y and enter if prompted about package versions)

```
termux-setup-storage; pkg upgrade -y && pkg install -y rust binutils python && pip install xdcc; mkdir -p ~/storage/shared/xdcc/progress ~/.termux/tasker/ && echo -e '#!/usr/bin/bash\nxdcc $1 send $2 | tee /storage/emulated/0/xdcc/progress/${1/|/.}-$2.txt' > ~/.termux/tasker/xdcc.sh
```
