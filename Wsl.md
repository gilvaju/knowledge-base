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