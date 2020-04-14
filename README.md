# Ubuntu-setup
### connect to online accounts
ubuntu single sign on

google

nextcloud


### apt
```sudo apt update```

```sudo apt-get install chromium-browser unity-tweak-tool htop python3-pip git vim exfat-utils exfat-fuse  python3-tk```

### github set usr and pw automatically
```git config --global user.name 'christianreiser'```

```git config --global user.password 'myPassword'```

### Ubuntu software store
```pomodoro```


### pip
```pip3 install --user numpy pandas tensorflow scikit-image Cython contextlib2 pillow lxml jupyter matplotlib```


### snap
```sudo snap install pycharm-community --classic```

```sudo snap install android-studio --classic```

```sudo snap install pdftk anki-woodrow audacity vlc gimp okular libreoffice```


#### next/cloud MAYBE BETTER FORM SOFTWARE CENTER: NEXTCLOUD CLIENT
```sudo add-apt-repository ppa:nextcloud-devs/client```

```sudo apt update```

```sudo apt install nextcloud-client```

### rescuetime
```wget https://www.rescuetime.com/installers/rescuetime_current_amd64.deb```

```sudo apt install ./rescuetime_current_amd64.deb```

```rescuetime```

```gabrielre1990@gmail.com```





### settings
(icon size, alt+del poweroff, workspaces,...)

```dconf dump / > mysettings.ini```

```dconf load / < mysettings.ini```

### autostart
move files to```~/.config/autostart```

### connect bt device [2C:41:A1:CA:5F:E0] with custom command [cb]
make file executable:
```chmod +x /home/chrei/code/Ubuntu-setup/scripts/autopairBose```

create alias (commandline abbreviation):
```
vim ~/.bashrc
alias cb='/home/chrei/code/Ubuntu-setup/scripts/autopairBose'
```

### screenlogger
install:
```sudo apt-get install scrot```

open/create file in vi:
```vi /home/chrei/code/Ubuntu-setup/scripts/screenlogger```

paste the following in the file:
```while true; do scrot -d 60 'screenLog%Y%m%d%H%M%S.jpg' -e 'mv $f /home/chrei/screenLogger/'; done```

close file
```:x```

make file executable:
```chmod +x /home/chrei/code/Ubuntu-setup/scripts/screenlogger```

create alias (commandline abbreviation):
```
vim ~/.bashrc
alias logs='/home/chrei/code/Ubuntu-setup/scripts/screenlogger'
```

refresh bashrc 
```source ~/.bashrc```


### keylogger (```https://github.com/kernc/logkeys/blob/master/INSTALL```)

```sudo apt-get update```
```sudo apt-get install autotools-dev autoconf```
```git clone https://github.com/kernc/logkeys.git && cd logkeys```
```./autogen.sh     # generate files for build```
```cd build  && ../configure```
```make```
``` sudo make install```
```git clean -xdf # clean```

open/create file in vi:
```vi /home/chrei/code/Ubuntu-setup/scripts/logkeys```

paste the following in the file:
```sudo logkeys -s --keymap=keymap_de --output=/home/chrei/screenLogger/keylogger/logkeys.log```

close file
```:x```

make file executable:
```chmod +x /home/chrei/code/Ubuntu-setup/scripts/logkeys```

create alias (commandline abbreviation):
```
vim ~/.bashrc
alias logk='/home/chrei/code/Ubuntu-setup/scripts/logkeys'
```

refresh bashrc 
```source ~/.bashrc```

