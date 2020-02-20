## dotfiles
used font: [Sarasa-Gothic](https://github.com/be5invis/Sarasa-Gothic)

### windows
* gvim path: `D:\Portable\Vim`

* dotfile path: `E:\Dropbox\dotfiles`

1. create `_vimrc` file
```bsh
git clone https://github.com/ovenx/dotfiles.git E:\Dropbox\Src\dotfiles
mklink "D:\Portable\Vim\_vimrc" E:\Dropbox\dotfiles\vimrc
```
2. use `plug.vim`. put `plug.vim` to D:\Portable\Vim\autoload, open gvim run `PlugInstall`

3. add explorer context menu. just run `edit-with-vim.reg`

4. modify `tagbar_ctags_bin` in _vimrc
```bash
let g:tagbar_ctags_bin='E:/Dropbox/Apps/ctags.exe'
```

### linux

1. create `vimrc` file
```bash
cd ~
git clone https://github.com/ovenx/dotfiles.git
ln -d ~/dotfiles/vimrc /usr/local/share/vim/vimrc
```

2. use `plug.vim`
```bash
cp ~/plug.vim /usr/local/share/vim/vim82/autoload/
```
open vim run PlugInstall