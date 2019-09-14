Title: centos-desktop-setting
Date: 2019-09-14 18:20
Modified: 2019-09-14 18:20
Category: centos
Tags: linux,centos,desktop
Slug: centos-desktop-setting
Authors: yjkim 
Summary: centos,desktop


# how to gnome desktop install 

```
gnome desktop install 
sudo yum update  
yum group list  
yum groupinstall "GNOME Desktop" "Graphical Administration Tools" 
ln -sf /lib/systemd/system/runlevel5.target /etc/systemd/system/default.target 
sudo reboot 
```

# tiger vnc install 

```
yum install tigervnc-server 
vncserver 
# geometry : resolution 
```