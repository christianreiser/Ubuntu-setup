# Ubuntu-setup
### connect to online accounts
ubuntu single sign on

google

nextcloud


### apt
sudo apt update

sudo apt-get install chromium-browser unity-tweak-tool htop python3-pip git vim exfat-utils exfat-fuse  python3-tk



### pip
pip3 install numpy pandas tensorflow


### snap
sudo snap install pycharm-community --classic


### detection api
pip3 install --user Cython contextlib2 pillow lxml jupyter matplotlib

mkdir code && cd code && git clone https://github.com/cocodataset/cocoapi.git

cd cocoapi/PythonAPI
make # error
cp -r pycocotools ~/code/models/research/
...

#### next/cloud MAYBE BETTER FORM SOFTWARE CENTER: NEXTCLOUD CLIENT
sudo add-apt-repository ppa:nextcloud-devs/client

sudo apt update

sudo apt install nextcloud-client




### settings
(icon size, alt+del poweroff, workspaces,...)

dconf dump / > mysettings.ini

dconf load / < mysettings.ini
