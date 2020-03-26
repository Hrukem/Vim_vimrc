# Vim_vimrc

set nocompatible              " be iMproved, required
filetype off                  " required

" set the runtime path to include Vundle and initialize
set rtp+=~/.vim/bundle/Vundle.vim
call vundle#begin()

Plugin 'VundleVim/Vundle.vim'
Plugin 'tpope/vim-fugitive'
Plugin 'rstacruz/sparkup', {'rtp': 'vim/'}

Plugin 'elixir-editors/vim-elixir'
Plugin 'preservim/nerdtree'
call vundle#end()            " required
filetype plugin indent on    " required
" To ignore plugin indent changes, instead use:
"filetype plugin on
"
" Brief help
" :PluginList       - lists configured plugins
" :PluginInstall    - installs plugins; append `!` to update or just :PluginUpdate
" :PluginSearch foo - searches for foo; append `!` to refresh local cache
" :PluginClean      - confirms removal of unused plugins; append `!` to auto-approve removal
"
" see :h vundle for more details or wiki for FAQ
" Put your non-Plugin stuff after this line
"
set nu
set ttimeoutlen=10 "Понижаем задержку ввода escape последовательностей
set tabstop=2
set linebreak
set dy=lastline
set ts=2
"set foldenable
"set fdm=indent
"set foldopen=all
"set autoindent
syntax on
set nobackup
set nowritebackup
set noswapfile
colorscheme desert
map <F2> <Esc>:NERDTree<CR>
set hls
inoremap jj <Esc>
set fileformat=unix
set guifont=Ubuntu\ Mono\ Bold\ 14
