# manjaro_init
KDE

1. hardcode-fix remove
2. optium-management
```
https://forum.manjaro.org/t/guide-install-and-configure-optimus-manager-for-hybrid-gpu-setups-intel-nvidia/92196
sudo pacman -S optimus-manager
yay -S optimus-manager-qt

sudo nano /etc/sddm.conf
#DisplayCommand
#DisplayStopCommand

Create autostart for optimus-manager-qt
Reboot
```

3. install programs
```
sudo pacman-mirrors -i -c China -m rank

sudo nano /etc/pacman.conf
[archlinuxcn]
SigLevel = Optional TrustedOnly
Server = https://mirrors.ustc.edu.cn/archlinuxcn/$arch

sudo pacman -Syy
sudo pacman -S archlinuxcn-keyring  
sudo pacman -Syyu

sudo pacman -S fcitx-im kcm-fcitx
sudo nano ~/.pam_environment

GTK_IM_MODULE=fcitx
QT_IM_MODULE=fcitx
XMODIFIERS=@im=fcitx

yay -S gtk2 easyconnect 
yay -S jetbrains-toolbox
yay -S v2ray qv2ray
sudo pacman -S postman evolution evolution-ews vim
```

