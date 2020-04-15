# dotfiles

All my personal dotfiles stored in one place

### First of all clone
```zsh
git clone https://github.com/rogern01/dotfiles.git ~/dotfiles
```

### Papirus Icon Theme
```zsh
wget -qO- https://raw.githubusercontent.com/PapirusDevelopmentTeam/papirus-icon-theme/master/install.sh | DESTDIR="$HOME/.icons" sh
```
After that open GNOME Tweak Tool and set the Icon Theme

## Terminator with zsh
#### installation

```zsh
sudo apt install terminator zsh curl ranger

# oh-my-zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

# oh-my-zsh plugins
git clone https://github.com/zsh-users/zsh-autosuggestions ~/.oh-my-zsh/custom/plugins/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-syntax-highlighting ~/.oh-my-zsh/custom/plugins/zsh-syntax-highlighting
# spaceship theme
git clone https://github.com/denysdovhan/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt"
ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"
```
#### link config
```zsh
ln -s ~/dotfiles/zsh/zshrc ~/.zshrc
ln -s ~/dotfiles/zsh/zsh_aliases ~/.zsh_aliases
ln -s ~/dotfiles/terminator ~/.config/terminator
```


