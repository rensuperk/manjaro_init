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
sudo pacman -S postman evolution evolution-ews vim zsh oh-my-zsh

sudo chsh -s /bin/zsh
git clone git://github.com/zsh-users/zsh-autosuggestions.git /usr/share/oh-my-zsh/plugins/zsh-autosuggestions
git clone git://github.com/zsh-users/zsh-syntax-highlighting.git /usr/share/oh-my-zsh/plugins/zsh-syntax-highlighting
cp /usr/share/oh-my-zsh/zshrc ~/.zshrc
nano ~/.zshrc
plugins=(git z zsh-autosuggestions zsh-syntax-highlighting)
source ~/.zshrc


ssh-keygen
config ssh maven vipkid.xml idea plugins tiger 
```

