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

# Batch/Bot Download
Download from either ARUTHA-BATCH (has older shows but takes a long time to load) or your chosen bot (has newest episodes as well as some older ones).

List almost every show available on [SubsPlease Packlist](https://subsplease.org/xdcc/) (over 1400!)

## Options

### Quality

|SD|720p|1080p|
|:-:|:-:|:-:|
|~300MB|~700MB|~1.2GB|

Default: `1080p`

### Directory

Set download directory

Default: `/storage/emulated/0/xdcc/`

### Choose Bot

Choose bot used to auto download

Default: `CR-HOLLAND|NEW`

### Update Rates

Choose how long between downloading bot/batch `.txt` files
 
Default: `12 hours` and `0.5 hours`
