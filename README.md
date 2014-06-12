## vim config for like310101

## Quick Start

1. Install Vundle:

   `$ git clone https://github.com/gmarik/Vundle.vim.git ~/.vim/bundle/Vundle.vim`

2. Configure Plugins:

   Put this at the top of your `.vimrc` to use Vundle. Remove plugins you don't need, they are for illustration purposes.

   ```vim
   set nocompatible              " be iMproved, required
   filetype off                  " required
   
   " set the runtime path to include Vundle and initialize
   set rtp+=~/.vim/bundle/Vundle.vim
   call vundle#begin()
   " alternatively, pass a path where Vundle should install plugins
   "call vundle#begin('~/some/path/here')
   
   " let Vundle manage Vundle, required
   Plugin 'gmarik/Vundle.vim'
   
   " The following are examples of different formats supported.
   " Keep Plugin commands between vundle#begin/end.
   " plugin on GitHub repo
   Plugin 'scrooloose/nerdtree'
   Plugin 'like310101/vim'
   Plugin 'kien/ctrlp.vim'
   Plugin 'tpope/vim-rails'
   Plugin 'MarcWeber/vim-addon-mw-utils'
   Plugin 'tomtom/tlib_vim'
   Plugin 'garbas/vim-snipmate'
   Plugin 'honza/vim-snippets'
   " plugin from http://vim-scripts.org/vim/scripts.html
   Plugin 'ack.vim'
   Plugin 'bundler.vim'
   Plugin 'c.vim'
   Plugin 'python.vim'
   Plugin 'bash-support.vim'
   " Git plugin not hosted on GitHub
   " Plugin 'git://git.wincent.com/command-t.git'
   " git repos on your local machine (i.e. when working on your own plugin)
   " Plugin 'file:///home/gmarik/path/to/plugin'
   " The sparkup vim script is in a subdirectory of this repo called vim.
   " Pass the path to set the runtimepath properly.
   " Plugin 'rstacruz/sparkup', {'rtp': 'vim/'}
   " Avoid a name conflict with L9
   " Plugin 'user/L9', {'name': 'newL9'}
   
   " All of your Plugins must be added before the following line
   call vundle#end()            " required
   filetype plugin indent on    " required
   " To ignore plugin indent changes, instead use:
   "filetype plugin on
   "
   " Brief help
   " :PluginList          - list configured plugins
   " :PluginInstall(!)    - install (update) plugins
   " :PluginSearch(!) foo - search (or refresh cache first) for foo
   " :PluginClean(!)      - confirm (or auto-approve) removal of unused plugins
   "
   " see :h vundle for more details or wiki for FAQ
   " Put your non-Plugin stuff after this line
   
   let mapleader=","
   
   "显示行号
   set nu
   
   " ctag config 
   set tag=tags;
   set autochdir
   
   "配色方案
   colorscheme custom
   
   "tab两个空格
   set ts=2
   set expandtab
   
   "打开ctrlp
   nmap <silent> <leader>f <C-p>

   ```

4. Install Plugins:

   Launch `vim` and run `:PluginInstall`

   To install from command line: `vim +PluginInstall +qall`

5. 配色方案:

   http://bytefluent.com/vivify/
