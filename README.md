whatot-vimrc
============

my vunble vimrc


##1.Install


```bash
if [ -f "~/.vimrc"  ]; then
  cp ~/.vimrc .vimrc-bakup
fi

mkdir -p ~/.vim/bundle/
git clone https://github.com/gmarik/vundle.git ~/.vim/bundle/vundle
git clone https://github.com/whatot/whatot-vimrc.git

cp whatot-vimrc/.vimrc ~/.vimrc
vim +BundleInstall +qa

'这个mru.vim是lilydjwg的修改版本,但还是有些许问题
cp mru.vim ~/.vim/bundle/mru.vim/plugin/mru.vim
cp whatot-vimrc/filenametags ~/.vim/
ctags -R -f ~/.vim/systags /usr/include /usr/local/include
```
