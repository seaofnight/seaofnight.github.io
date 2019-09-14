Title: manjaro-local-setting
Date: 2019-09-14 18:20
Modified: 2019-09-14 18:20
Category: local
Tags: local
Slug: manjaro-local-setting
Authors: yjkim 
Summary: local

# oh-my-zsh install 

chsh -s `which zsh`
echo $SHELL 
curl -L https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh | sh

# theme change 
# terminal 환경에서  안깨지는 font 적용 후 확인  

# zsh autosuggestion install 


# byobu install 
 
git clone https://aur.archlinux.org/byobu.git
cd byobu
makepkg
pacman -U *.xz

# kvm install

LC_ALL=C lscpu | grep Virtualization
Virtualization: VT-x
sudo pacman -S virt-manager qemu vde2 ebtables dnsmasq bridge-utils openbsd-netcat
sudo systemctl enable libvirtd.service
sudo systemctl start libvirtd.service
 
# virtualbox install 

sudo pacman -S virtualbox virtualbox-ext-vnc virtualbox-guest-dkms virtualbox-host-dkms virtualbox-guest-utils virtualbox-guest-iso virtualbox-sdk 

yjkim@yjkim-pc  ~/문서  uname -r
4.19.66-1-MANJARO
sudo pacman -S linux419-virtualbox-host-modules

# vscode hangul encodding 

type [Ctrl + ,]
* linux default terminal 에서 한글이 출력되는 font 로 변경 필요 
setting > editor.fontFamily : ""DejaVu Sans Mono for Powerline""



# shutdown freeze solving

https://forum.manjaro.org/t/how-to-troubleshoot-shutdown-delays/5767

# install other package 

jq, tree

# firefox extension 

* translate

# linux application remove password prompt 

* docker 
sudo usermod -a -G docker $USER

* libvirtd, virt-manager 
sudo usermod -a -G libvirt $USER


# python pip install on manjaro 

```
python2 --version
Python 2.7.16
python3 --version
Python 3.7.4

sudo pacman -S python-pip --noconfirm

```