## arch bspwm的配置指南

这里主要是使用别人的脚本

首先配置一下raw.githubusercontent.com

sudo vim /etc/hosts
加入以下内容

```
185.199.108.113  raw.githubusercontent.com
185.199.109.113  raw.githubusercontent.com
185.199.110.113  raw.githubusercontent.com
185.199.111.113  raw.githubusercontent.com

```

**配置一下yay**

```bash
sudo pacman -S git base-devel
cd ~
mkdir -p .local
mkdir -p .local/opt
cd .local/opt
git clone https://aur.archlinux.org/yay-bin.git
cd yay-bin
makepkg -si
```

接着使用以下内容

```
curl https://raw.githubusercontent.com/gh0stzk/dotfiles/master/RiceInstaller -o $HOME/RiceInstaller

chmod +x RiceInstaller

./RiceInstaller
```

## 配置hyprland

```bash
git clone https://github.com/SolDoesTech/HyprV2.git
```
找到里面的set-hypr然后执行

这大概率会失败，主要是网络问题

试试这个hyprland

```bash
https://github.com/JaKooLit/HyprLanD.git
 chmod +x paru-hyprland
```

