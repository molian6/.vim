## Dotvim

These are my dotvim files that I use in my daily development. I have for long used a modified version of
spf13 with heavy customizations on top of it. But with time, it felt a bit sluggish and heavy. So decided
to start my .vimrc from scratch. The following config is a direct result of this. It feels very fast and it
is fun to write code in my Vim again. Hope you enjoy it and if you do, you can tip me here at https://gratipay.com/vinitkme/. Thanks! :)

## Installation:

In order to install the latest version:

```sh
git clone https://github.com/pingzh/.vim.git
git clone https://github.com/gmarik/Vundle.vim.git ~/.vim/bundle/Vundle.vim
cd .vim
mkdir ~/.vim/colors #if you don't have colors directory
cp colors/* ~/.vim/colors/
ln -s vimrc ~/.vimrc
vim +BundleInstall +qall

## Here I personally use RailsCasts


--Some solutions to bugs

1. If you see '$' at the end of each line, you just comment row 96, set list

2. If you get an error, like "VIM Error: E474: Invalid argument: listchars=tab:»·,trail:·", then you put the following two lines on the top of vimrc file:

scriptencoding utf-8
set encoding=utf-8
