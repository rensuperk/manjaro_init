# manjaro_init
KDE
sudo pacman-mirrors -i -c China -m rank

hardcode-fix remove

/etc/pacman.conf
`
[archlinuxcn]
SigLevel = Optional TrustedOnly
Server = https://mirrors.ustc.edu.cn/archlinuxcn/$arch
`
sudo pacman -Syy
sudo pacman -S archlinuxcn-keyring  


fcitx-im fcm-fcitx
```
~/.pam_environment

GTK_IM_MODULE=fcitx
QT_IM_MODULE=fcitx
XMODIFIERS=@im=fcitx
```
easyconnect
yay -S gtk2 easyconnect jetbrains-toolbox

