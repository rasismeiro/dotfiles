# dotfiles

## Installation:

```
git clone git://github.com/falmp/dotfiles.git ~/.dotfiles
cd ~/.dotfiles
git submodule update --init
.bin/bootstrap
```

## Update:

```
cd ~/.dotfiles
git pull
git submodule update --init
```

## Installation of vim plugins:

```
cd ~/.dotfiles
git submodule add https://github.com/tpope/vim-pathogen.git .vim/bundle/pathogen
git add .
git commit -m "Install pathogen"
git push
```

## Uninstallation of vim plugins:

```
cd ~/.dotfiles
git submodule deinit -f .vim/bundle/nerdtree
git rm -f .vim/bundle/nerdtree # use --cached instead to keep files
git add .
git commit -m "Uninstall nerdtree"
git push
```
