## Requirements:
* vim
* vim-gtk3 (gvim)

## Installation:
`git clone git@github.com:n0nnnnc/.vim.git ~/.vim`

## Create symlinks:
```
ln -s ~/.vim/vimrc ~/.vimrc
ln -s ~/.vim/gvimrc ~/.gvimrc
```

## Switch to the ~/.vim directory, and fetch submodules:
```
cd ~/.vim
git submodule init
git submodule update
```

## Upgrading a plugin bundle.
At some point in the future, the plugin might be updated. To fetch the latest changes, go into the plugin repository, and pull the latest version:
```
cd ~/.vim/bundle/dracula
git pull origin main
```

## Upgrading all bundled plugins
You can use the foreach command to execute any shell script in from the root of all submodule directories. To update to the latest version of each plugin bundle, run the following:
```
git submodule foreach git pull origin master
```
