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
create scrips dir:
```mkdir -p ~/scripts```

open/create file in vi:
```vi ~/scripts/autopair```

paste the following in the file:
```#!/bin/bash
bluetoothctl << EOF
connect 2C:41:A1:CA:5F:E0
EOF```

close file
```:x```

make file executable:
```chmod +x ~/scripts/autopair```

create alias (commandline abbreviation):
```vim ~/.bashrc
alias cb='~/scripts/autopair'```

close file
:x

### screenlogger
install:
```sudo apt-get install scrot```

open/create file in vi:
```vi ~/scripts/screenlogger```

paste the following in the file:
```while true; do scrot -d 60 'screenLog%Y%m%d%H%M%S.jpg' -e 'mv $f ~/screenLogger/'; done```

close file
```:x```

make file executable:
```chmod +x ~/scripts/screenlogger```

add to startup application:
open ```startup applications```
paste ```~/scripts/screenlogger``` as command

