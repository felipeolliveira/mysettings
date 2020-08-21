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
## Yarn install

```
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list

sudo apt update && sudo apt install --no-install-recommends yarn
```

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
```

After all, copy files from folder `shell_config_files` to home directory `~/`

# Configuration Git, Hyper and ZSH

## SSH conection:

- Access github ssh setting and configure ssh for your client

## Clone this repo:

```
git clone git@github.com:felipeolliveira/mysettings.git ~/.mysettings
```

## Apply configuration files:

- remove `.zshrc` `.hyper.js` `.gitconfig` and create symbolic links to home directory `~/`

```
rm -f ~/.zshrc ~/.hyper.js ~/.gitconfig && ln -s ~/.mysettings/shell_config_files/.zshrc ~/.zshrc && ln -s ~/.mysettings/shell_config_files/.hyper.js ~/.hyper.js && ln -s ~/.mysettings/shell_config_files/.gitconfig ~/.gitconfig
```

# VS-Code

- Sync with extension `Settings Sync`
- If you have visual glitches, paste in json file `Configure Runtime Arguments`, access for command pallet:

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
