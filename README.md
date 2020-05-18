# My .vimrc File -- Lucas Pichette

" You can copy and paste this or download it, C&P is probably easiest.

" Don't try to be vi compatible          
set nocompatible     

" Helps force plugins to load correctly when it is turned back on below          
filetype off     

" This the first key we press when we start our own personalized mappings, remember it as 'leader'
set mapleader=','

" Plugins {{{     
call plug#begin('~/vimfiles/')     

Plug ('morhetz/gruvbox') " Call :PlugInstall for first time adding this .vimrc

call plug#end()     
" Use :PlugInstall and :PlugUpdate for vim-plug, put plug.vim into vimfiles/autoload (if no autoload directory make autoload directory)     
" }}}     

" File Config {{{     
filetype plugin indent on " For plugins to load correctly     
" }}}     

" Aesthetics {{{     
set visualbell     
set vb t_vb=     
set t_Co=256 "Sets terminal color pallete to be 256     
set background=dark     
let g:gruvbox_termcolors=256     
let g:gruvbox_transparent_bg=1     
colorscheme gruvbox     
set listchars=tab:▸\ ,eol:¬      
" set list " To enable listchars default      
map <leader>l :set list!<CR> "Toggles list chars by pressing <,-l>, where <,-l> means: 'press comma *then* l' 
" }}}     

" Utility {{{     
set number     
set ruler     
syntax on " Turn on syntax highlighting     
" }}}     

" Encoding {{{
set encoding=utf-8
" }}}

" Whitespace {{{     
set wrap     
set textwidth=79     
set formatoptions=tcqrn1     
set tabstop=2     
set shiftwidth=2     
set softtabstop=2     
set expandtab     
set noshiftround     
" }}}     

" Keybindings {{{     
set scrolloff=8 "Creates an offset of 8 lines at the top of your screen     
set backspace=indent,eol,start     
" }}}     

" Mappings {{{     
     
" }}}     

" Optimization {{{     
set ttyfast     
set lazyredraw     
" }}}     

" Status Line {{{     
set laststatus=2 "Makes status line static      
set showmode "Shows insert/replace/visual-line/etc in status line     
set showcmd "Shows current command in status line     
" }}}     

" Searching {{{     
set hlsearch     
set incsearch     
set ignorecase     
set smartcase     
set showmatch     
" }}}     
