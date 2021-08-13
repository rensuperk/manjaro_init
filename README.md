# manjaro_init
KDE

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
sudo pacman -S postman evolution evolution-ews vim zsh oh-my-zsh docker docker-compose timeshift stacer

sudo chsh -s /bin/zsh
git clone git://github.com/zsh-users/zsh-autosuggestions.git /usr/share/oh-my-zsh/plugins/zsh-autosuggestions
git clone git://github.com/zsh-users/zsh-syntax-highlighting.git /usr/share/oh-my-zsh/plugins/zsh-syntax-highlighting
cp /usr/share/oh-my-zsh/zshrc ~/.zshrc
nano ~/.zshrc
plugins=(git z zsh-autosuggestions zsh-syntax-highlighting)
source ~/.zshrc


sudo usermod -aG docker ${USER}
sudo systemctl start docker
sudo systemctl enable docker
su root             切换到root用户
su ${USER}          再切换到原来的应用用户以上配置才生效

ssh-keygen
config ssh maven vipkid.xml idea plugins tiger 
```
