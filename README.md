# Ubuntu-setup
### connect to online accounts
ubuntu single sign on

google

nextcloud


### apt
```sudo apt update```

```sudo apt-get install chromium-browser unity-tweak-tool htop python3-pip git vim exfat-utils exfat-fuse  python3-tk```



### pip
```pip3 install --user numpy pandas tensorflow scikit-image Cython contextlib2 pillow lxml jupyter matplotlib```


### snap
```sudo snap install pycharm-community --classic```


#### next/cloud MAYBE BETTER FORM SOFTWARE CENTER: NEXTCLOUD CLIENT
```sudo add-apt-repository ppa:nextcloud-devs/client```

```sudo apt update```

```sudo apt install nextcloud-client```




### settings
(icon size, alt+del poweroff, workspaces,...)

```dconf dump / > mysettings.ini```

```dconf load / < mysettings.ini```

### connect bt device [2C:41:A1:CA:5F:E0] with custom command [cb]
```mkdir -p ~/scripts```
```vi ~/scripts/autopair```

```#!/bin/bash
bluetoothctl << EOF
connect 2C:41:A1:CA:5F:E0
EOF```

```:x```
```chmod +x ~/scripts/autopair```
```alias cb='~/scripts/autopair'```
