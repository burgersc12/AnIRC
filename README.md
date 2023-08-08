AnimeXD - Auto Download Anime


# Guide to xdcc install

## Step 1: Download plugins

[Termux](https://www.f-droid.org/packages/com.termux/)

[Termux:Tasker](https://www.f-droid.org/packages/com.termux.tasker/)

## Step 2: Paste this into Termux
```
termux-setup-storage; pkg upgrade -y && pkg install -y rust binutils python && pip install xdcc; mkdir -p ~/storage/shared/xdcc/progress ~/.termux/tasker/ && echo -e '#!/usr/bin/bash\nxdcc $1 send $2 | tee /storage/emulated/0/xdcc/progress/${1/|/.}-$2.txt' > ~/.termux/tasker/xdcc.sh
```
Make sure to allow files permissions. Hit y and enter if prompted about package versions, this will download the latest version of each package.

# Batch/Bot Download Info
Download from either ARUTHA-BATCH, which has older shows but takes a long time to load, or default bot.

Lists almost every show available on [SubsPlease Packlist](https://subsplease.org/xdcc/)

# Settings

### Quality

|SD|720p|1080p|
|:-:|:-:|:-:|
|~400MB|~700MB|~1.4GB|

Default: `1080p`

### Directory

Set download directory

Default: `/storage/emulated/0/xdcc/`

### Choose Bot

Choose bot used to auto download

Default: `CR-HOLLAND|NEW`

### Update Rates

Choose how long between downloading batch and bot `.txt` files
 
Default: `12 hours` and `0.5 hours`
