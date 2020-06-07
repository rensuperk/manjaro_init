# manjaro_init
KDE

1. hardcode-fix remove
2. install programs
```
sudo pacman-mirrors -i -c China -m rank

sudo nano /etc/pacman.conf
[archlinuxcn]
SigLevel = Optional TrustedOnly
Server = https://mirrors.ustc.edu.cn/archlinuxcn/$arch

sudo pacman -Syy
sudo pacman -S archlinuxcn-keyring  
sudo pacman -Syyu

sudo pacman -S fcitx-im fcm-fcitx
sudo nano ~/.pam_environment

GTK_IM_MODULE=fcitx
QT_IM_MODULE=fcitx
XMODIFIERS=@im=fcitx

yay -S gtk2 easyconnect 
yay -S jetbrains-toolbox
yay -S v2ray qv2ray
```

