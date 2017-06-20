# 基本系統設定

### [1]更新Ubuntu

sudo apt-get update && sudo apt-get upgrade

若遇到問題，依指示sudo apt-get -f install

### [2]安裝新酷音

先去language選項內安裝traditional Chinese

sudo apt-get install ibus-chewing

將中文的優先權調至最高並重新登入，將輸入法中新增ibus新酷音

### [3]匯入firefox書籤頁

Bookmarks -> Show All Bookmarks -> Import and Backup -> Restore -> Choose File...

### [4]整理Launcher Bar

只留下Files, Firefox, Software, Amazon, Settings, Spotify, Terminal, Atom, Trash

### [5]記得將系統語言設定為English

# 套件&軟體設定

### [1]安裝vim

sudo apt-get install vim

### [2]安裝git

sudo apt-get install git

### [3]安裝Atom

到 atom.io下載 atom-xxx.deb

sudo dpkg -i xxx.deb

atom.io packages for web-dev:
- apm install atom-html-preiew
- apm install csscomb
- apm install color-picker
- apm install atom-beautify

### [4]安裝Dropbox

go to https://www.dropbox.com/install-linux

follow instructions

若是出現警告要求restart Nautilus: sudo nautilus -q

### [5]安裝spotify :p

go to https://www.spotify.com/tw/download/linux/

follow the instructions

### [6]安裝Flash player for watching Safari Online Video

sudo apt-get install flashplugin-installer

# Python 3.6 開發環境

### 參考網址：
- https://www.openfoundry.org/tw/tech-column/8516-pythons-virtual-environment-and-multi-version-programming-tools-virtualenv-and-pythonbrew
- https://www.howopensource.com/2011/05/installation-of-virtualenv-in-linux/
- https://stackoverflow.com/questions/42662104/how-to-install-pip-for-python-3-6-on-ubuntu-16-10/44254088#44254088

### 安裝Python3.6：
- sudo add-apt-repository ppa:jonathonf/python-3.6
- sudo apt update
- sudo apt install python3.6
- sudo apt install python3.6-dev
- sudo apt install python3.6-venv
- wget https://bootstrap.pypa.io/get-pip.py
- sudo python3.6 get-pip.py

(optional)
- sudo ln -s /usr/bin/python3.6 /usr/local/bin/python
- sudo ln -s /usr/bin/python3.6 /usr/local/bin/python3
- sudo ln -s /usr/local/bin/pip /usr/local/bin/pip3

### 安裝virtualenv：
- sudo apt-get install python-setuptools
- sudo easy_install virtualenv
- virtualenv --no-site-packages --python=python3.6 path/to/our/[環境名稱]

### 進入/退出環境：
- cd path/to/our/[環境名稱]
- (進入)source bin activate
- (退出)deactivate
