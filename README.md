sudo apt install vim-gui-common
sudo apt install vim-runtime
mkdir -p ~/.vim/pack/vendor/start
git clone --depth 1 \ https://github.com/preservim/nerdtree.git \ ~/.vim/pack/vendor/start/nerdtree
git clone --depth 1 \ https://github.com/PhilRunninger/nerdtree-buffer-ops.git \ ~/.vim/pack/vendor/start/nerdtree/nerdtree_plugin
git clone --depth 1 \ https://github.com/scrooloose/nerdtree-project-plugin.git \ ~/.vim/pack/vendor/start/nerdtree/nerdtree_plugin
git clone --depth 1 \ https://github.com/tpope/vim-commentary.git \ ~/.vim/pack/vendor/start/commentary


.vimrc:

set nocompatible
filetype on
filetype plugin on
filetype indent on
set number

syntax on

nnoremap ä :NERDTreeToggle
nnoremap ö :NERDTree

:hi Normal ctermfg=Red ctermbg=Black
