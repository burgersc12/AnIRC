# Installation Instructions

Install [Termux](https://f-droid.org/en/packages/com.termux/) and [Termux:Tasker](https://f-droid.org/en/packages/com.termux.tasker/)

### Commands to run in Termux

```
pkg update && pkg install -y python && pip install xdcc-dl && mkdir -p ~/.termux/tasker/ ; termux-setup-storage
```

```
echo -e '#!/usr/bin/bash\ncd $3\nxdcc-dl "/msg $1 xdcc send #$2" | tee -a .stdout.txt' > ~/.termux/tasker/xdcc-dl.sh && sed -i 's/columns = 80/columns = 1000/g' ~/../usr/lib/python3.10/site-packages/xdcc_dl/xdcc/XDCCClient.py
```

**Tap Command To Show Copy Button**

## App Permissions to Allow

`Storage`

`Run commands in Termux environment`

`Draw over other apps`

**NOTE**

.apk file can be found under [Releases](https://github.com/burgersc12/AnIRC/releases)
