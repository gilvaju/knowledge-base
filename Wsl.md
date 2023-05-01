```
https://youtu.be/sjrW74Hx5Po
https://wsldl-pg.github.io/ArchW-docs/How-to-Setup/

pacman -S --needed git base-devel && git clone https://aur.archlinux.org/yay.git && cd yay && makepkg -si

yay -S asdf-vm fish starship
mkdir ~/.config/fish

echo set fish_greeting > ~/.config/fish/config.fish && echo source /opt/asdf-vm/asdf.fish >> ~/.config/fish/config.fish && echo "starship init fish | source" >> ~/.config/fish/config.fish

wsl -d ArchWslBase -u gilvaju --cd ~

yay -S docker ansible docker-compose python-docker python-pip libxcrypt-compat python-setuptools

sudo usermod -aG docker $USER
sudo systemctl start docker
sudo systemctl enable docker


```

https://www.nerdfonts.com/font-downloads
Na pasta do usuário:  .wslconfig

```
[wsl2]
memory=13GB
processors=6
swap=2GB

Chocolatey

choco install obsidian discord vscode
```

```
#### Setup ubuntu distro
#!/bin/bash 
sudo apt update 
	&& sudo apt upgrade -y 
	&& sudo apt install automake unzip curl build-essential autoconf fish nano git htop -y
```

```
sudo add-apt-repository ppa:neovim-ppa/unstable
sudo apt-get update
sudo apt-get install neovim
```

```
chsh -s /usr/bin/fish 
	&& mkdir ~/.config 
	&& mkdir ~/.config/fish 
	&& touch ~/.config/fish/config.fish
	&& mkdir -p ~/.config/fish/completions 
	&& sleep 5s 
	&& echo "set fish_greeting" >> ~/.config/fish/config.fish
```

```
curl -sS https://starship.rs/install.sh | sh 
	&& echo "starship init fish | source" >> ~/.config/fish/config.fish 
```

```
git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.10.2 
	&& echo "source ~/.asdf/asdf.fish" >> ~/.config/fish/config.fish
	&& ln -s ~/.asdf/completions/asdf.fish ~/.config/fish/completions
```

```
cp -r /mnt/c/Users/gilvaju/Downloads/.ssh/ ~/.ssh 
	&& chmod 600 ~/.ssh/id_ed25519 ~/.ssh/comigo.pem ~/.ssh/comigo-admin.pem
```

```
`#!/bin/bash    
asdf plugin add nodejs https://github.com/asdf-vm/asdf-nodejs.git 
	&& asdf install nodejs latest 
	&& asdf install nodejs 16.14.2 
	&& asdf global nodejs latest 
	&& asdf reshim 
	&& corepack enable 
	&& asdf reshim 
	&& yarn -v
```

```
cd ~ && mkdir projects && cd projects && git clone git@github.com:comigotech/comigo.git`
ssh -i ~/.ssh/comigo.pem ubuntu@go.semprecomigo.com.br
```

```
wsl --import UbuntuTeste ./UbuntuTeste ubuntu-default.zip

wsl --export Ubuntu ubuntu-default.zip
```

```
### Method 1 - `/etc/wsl.conf`

The current [Microsoft recommended](https://docs.microsoft.com/en-us/windows/wsl/wsl-config#user-settings) way of setting the username in an instance is to create a `/etc/wsl.conf` in the instance with the following setting:

[user]
default=username
```

```
[boot] systemd=true
```

```
 wsl -d Ubuntu --cd ~
```

```
sudo usermod -aG docker $USER
```

```
sudo update-alternatives --set iptables /usr/sbin/iptables-legacy
sudo update-alternatives --set ip6tables /usr/sbin/ip6tables-legacy
```

```
**

choco install googlechrome 7zip spotify discord steam epicgameslauncher goggalaxy google-drive-file-stream ChocolateyGUI virtualbox clavier-plus rufus obsidian github-desktop  -y

winget install --id Microsoft.Powershell --source winget

—-----------------------------------------------------------------------------

cd D:\

mkdir WSL
cd WSL
mkdir Ubuntu
wsl --export Ubuntu .\Ubuntu\ext4.vhdx --vhd
wsl --unregister Ubuntu
wsl --import-in-place Ubuntu .\Ubuntu\ext4.vhdx

wsl -d Ubuntu -u gilvaju

**
```


```
**  

# sudo nano /etc/pacman.conf
# ParallelDownload = 15
sudo pacman-mirrors -f && sudo pacman -Syyu
sudo pacman -S --needed base-devel fish git pavucontrol pulseaudio timeshift yay

yay -S discord obsidian google-chrome sublime-text-4 jetbrains-toolbox spotify-launcher asdf-vm github-cli microsoft-edge-stable-bin

mkdir ~/.config/fish

echo set fish_greeting > ~/.config/fish/config.fish
echo source /opt/asdf-vm/asdf.fish >> ~/.config/fish/config.fish
echo "starship init fish | source" >> ~/.config/fish/config.fish

# ~/.zshrc
# . /opt/asdf-vm/asdf.sh
chmod 600 ~/.ssh/comigo-admin.pem ~/.ssh/comigo.pem ~/.ssh/id_ed25519.pub ~/.ssh/id_ed25519
mkdir -p ~/Projetos/comigo && mkdir -p ~/Projetos/ycodify
gh auth login

asdf install nodejs 18.14.0 && asdf global nodejs 18.14.0 && corepack enable && asdf reshim
npm install --global hasura-cli serverless

# https://stackoverflow.com/questions/7446187/no-module-named-pkg-resources
sudo pacman -S docker docker-compose python-docker python-pip ansible libxcrypt-compat python-setuptools
sudo systemctl enable docker.service
sudo usermod -aG docker $USER
# REINICIAR O COMPUTADOR

—-----------------------------------------------------------------------------

cp -r /mnt/c/Users/gilvaju/Downloads/.ssh/ ~/.ssh
chmod 600 ~/.ssh/id_ed25519 ~/.ssh/comigo.pem
rm ~/.ssh/known_hosts
ssh -i ~/.ssh/comigo.pem [ubuntu@go.semprecomigo.com.br](mailto:ubuntu@go.semprecomigo.com.br)

—-------------------------------------------------------------------------

sudo pacman -S --needed git base-devel fish gitflow-avh fontconfig openssh docker docker-compose ttf-fira-code htop
# [https://github.com/Jguer/yay](https://github.com/Jguer/yay)
git clone https://aur.archlinux.org/yay.git && cd yay && makepkg -si
sudo apt update && sudo apt upgrade -y
sudo apt install automake unzip curl build-essential autoconf fish nano git-flow htop -y

—---------------------------------

WAYLAND_DISPLAY=“wayland-1” / set WAYLAND_DISPLAY “wayland-1”
setxkbmap -model abnt2 -layout br -variant abnt2 / sudo apt install x11-xkb-utils
WAYLAND_DISPLAY=“wayland-1” / set WAYLAND_DISPLAY “wayland-1”
**
```