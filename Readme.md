# Shell Config

## Zsh

```
sudo apt install wget curl git -y
sudo apt install zsh
sudo usermod -s $(which zsh) <username>

zsh --version
echo $SHELL
```

## Oh-my-Zsh

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

## Hyper

Download in [Hyper's website](https://hyper.is/#installation):

```
sudo apt install ~/Downloads/<hyper.deb>
```

## Fira Code

```
sudo apt install fonts-firacode
```

## Spaceship theme

```
# Download spaceship theme into oh-my-zsh theme folder

git clone https://github.com/denysdovhan/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt"

#create a symbolic link to spaceship

ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"
```

## ZInit - plugins for zsh

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/zdharma/zinit/master/doc/install.sh)"
```

## Set default terminal to Hyper

```
which hyper

sudo update-alternatives --install /usr/bin/x-terminal-emulator x-terminal-emulator <hyper path> 0

sudo update-alternatives --set x-terminal-emulator <hyper path>
```

## NVM install

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
```

After all, copy files from folder `shell_config_files` to home directory `~/`

# Git config

- Access github ssh setting and configure ssh for client

# VS-Code

- Sync with extension `Settings Sync`
- If have visual glitches, paste in json file `Configure Runtime Arguments`, access for command pallet:

```
"force-color-profile": "srgb",
```

# Appearance

## apps

```
sudo apt install gnome-tweaks
```

## theme

```
sudo apt install sassc -y

git clone --depth 1 https://github.com/nana-4/materia-theme

cd ./materia-theme/

sudo ./install.sh

cd ..

rm -rf ./materia-theme/
```

## Icons

```
git clone https://github.com/vinceliuice/Tela-icon-theme.git\

cd ./Tela-icon-theme/

sudo ./install.sh <color>

cd ..

rm -rf ./materia-theme/
```

## Cursor

[PearWhiteCursor](https://www.gnome-look.org/p/1327310/)

```
sudo mv ~/Downloads/PearWhiteCursors /usr/share/icons
```
