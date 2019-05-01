# Ubuntu-setup
### connect to online accounts
ubuntu single sign on

google

nextcloud

### programs
sudo apt update

sudo apt-get install chromium-browser

sudo apt install unity-tweak-tool

sudo apt install htop

sudo apt install python3-pip

%sudo apt install python-pip

sudo apt install git

sudo apt-get install exfat-utils exfat-fuse 




### pip
pip3 install numpy

pip3 install tensorflow


### detection api
pip3 install --user Cython
pip3 install --user contextlib2

pip3 install --user pillow

pip3 install --user lxml

pip3 install --user jupyter

pip3 install --user matplotlib

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
