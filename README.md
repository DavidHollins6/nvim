# David's Dotfiles

Somewhere for me to keep all of my dotfiles while I build a better developer workflow for myself.

## Alacritty

Sym link the config.

`ln -s ~/dotfiles/alacritty/alacritty.yml ~/.config/alacritty.yml`

Download the Mononoki Nerd Font. [This](https://www.nerdfonts.com/font-downloads) is a good place to find it.


## TMUX

Ensure `tmux` is installed.

`brew install tmux`

Symlink it.

`ln -s ~/dotfiles/tmux/.tmux.conf ~/.tmux.conf`

## ZSH

Symlink the zsh config.

`ln -s ~/dotfiles/zsh/.zshrc ~/.zshrc`

## NVIM

Based off [The Primeagens NVIM Configuration](https://github.com/ThePrimeagen/init.lua) 

Clone this repository into you home directory.

```
cd ~

git init
git remote add origin git@github.com:DavidHollins6/dotfiles.git
git pull origin main
```

Make sure to [install packer](https://github.com/wbthomason/packer.nvim#quickstart)

Source your files

```
:so
```

Install packer plugins

```
:PackerSync
```

Restart vim
