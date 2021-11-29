---
layout: post
author: ted
---
ubuntu-16.04.7-server-amd64

1.vi  
ubuntu@ubuntu:~$ sudo vi /etc/vim/vimrc.tiny  
ubuntu@ubuntu:~$ sudo vi .vimrc
```
set nocompatible
set backspace=2
set nu
set tabstop=4
set expandtab
set softtabstop=4
```

2.samba  
ubuntu@ubuntu:~$ vi /etc/samba/smb.conf  
```
passdb backend = tdbsam  
[ubuntu]  
comment = Home  
path = /home/ubuntu  
browseable = yes  
read only = no  
valid users = ubuntu
```
ubuntu@ubuntu:~$ sudo pdbedit -a ubuntu  

3.apt
ubuntu@ubuntu:~$ sudo vi /etc/apt/sources.list  
mirror: <https://mirrors.tuna.tsinghua.edu.cn/help/ubuntu/>  

win10

1.gvim  
vim: <https://www.vim.org/>  
truvbox: <https://github.com/morhetz/gruvbox>  
C:\\Program Files \(x86\)\\Vim\>vim _vimrc  
```
winpos 150 150  
set lines=35 columns=120  
set nocompatible  
set backspace=2  
set nu  
set tabstop=4  
set expandtab  
set softtabstop=4  
set nolist  
set guioptions-=T  
set guioptions-=m  
set guioptions-=l  
set guioptions-=L  
set guioptions-=r  
set guioptions-=R  
set nobackup  
set noswapfile  
set nowritebackup  
set noundofile  
set encoding=utf-8  
set termencoding=utf-8  
set fileencodings=ucs-bom,utf-8,chinese,cp936  
language messages zh_CN.utf-8  
source $VIMRUNTIME/delmenu.vim  
source $VIMRUNTIME/menu.vim  
colorscheme gruvbox  
set guifont=Consolas:h12:cANSI  
```
2.sshfs  
<https://github.com/billziss-gh/sshfs-win>  
<https://github.com/billziss-gh/winfsp>  
\\\\sshfs\sdk@172.28.48.112\ 

