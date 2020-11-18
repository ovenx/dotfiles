# dotfiles

## vim

used font: [Sarasa-Gothic](https://github.com/be5invis/Sarasa-Gothic)

### windows
1. create `vimrc` file
```bash
cd d:/
git clone https://github.com/ovenx/dotfiles.git
mklink "path_to_gvim\vimrc" d:\dotfiles\vimrc
```
2. install vim-plug, open gvim run `PlugInstall`

```powershell
iwr -useb https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim |`
    ni "$env:LOCALAPPDATA/nvim-data/site/autoload/plug.vim" -Force
```

3. add explorer context menu. just run `edit-with-vim.reg`

4. modify `tagbar_ctags_bin` in `_vimrc`
```bash
https://github.com/universal-ctags/ctags-win32/releases
let g:tagbar_ctags_bin='path_to_ctags/ctags.exe'
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
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```
3. open vim run PlugInstall
