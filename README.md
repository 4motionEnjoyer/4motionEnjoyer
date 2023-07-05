sudo apt install vim-gui-common

sudo apt install vim-runtime

mkdir -p ~/.vim/pack/vendor/start

git clone --depth 1 https://github.com/preservim/nerdtree.git ~/.vim/pack/vendor/start/nerdtree

git clone --depth 1 https://github.com/PhilRunninger/nerdtree-buffer-ops.git ~/.vim/pack/vendor/start/nerdtree/nerdtree_plugin

git clone --depth 1 https://github.com/scrooloose/nerdtree-project-plugin.git ~/.vim/pack/vendor/start/nerdtree/nerdtree_plugin

git clone --depth 1 https://github.com/tpope/vim-commentary.git ~/.vim/pack/vendor/start/commentary/

git clone --depth 1 https://github.com/jiangmiao/auto-pairs.git ~/.vim/pack/vendor/start/autopair/



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





.config/tickrs/config.yaml:


#/ List of ticker symbols to start app with
symbols:
  - NOKIA.HE
  - TLT1V.HE
  - FIA1S.HE

#/ Chart type to start app with
#/ Default is line
#/ Possible values: line, candle, kagi
chart_type: line

#/ Use specified time frame when starting program and when new stocks are added
#/ Default is 1D
#/ Possible values: 1D, 1W, 1M, 3M, 6M, 1Y, 5Y
#time_frame: 1D

#/ Interval to update data from API (seconds)
#/ Default is 1
#update_interval: 1

#/ Enable pre / post market hours for graphs
enable_pre_post: true

#/ Hide help icon in top right
#/hide_help: true

#/ Hide previous close line on 1D chart
#hide_prev_close: true

#/ Hide toggle block
#hide_toggle: true

#/ Show volumes graph
show_volumes: true

#/ Show x-axis labels
show_x_labels: true

#/ Start in summary mode
#summary: true

#/ Truncate pre market graphing to only 30 minutes prior to markets opening
#trunc_pre: true

#/ Ticker options for Kagi charts
#
#/ A map of each ticker with reversal and/or price fields (both optional). If no
#/ entry is defined for a symbol, a default of 'close' price and 1% for 1D and 4%
#/ for non-1D timeframes is used. This can be updated in the GUI by pressing 'e'
#
#/ reversal can be supplied as a single value, or a map on time frame to give each
#/ time frame a different reversal amount
#
#/ reversal.type can be 'amount' or 'pct'
#
#/ price can be 'close' or 'high_low'
#
#kagi_options:
#/  SPY:
#/    reversal:
#/      type: amount
#/      value: 5.00
#/    price: close
#/  AMD:
#/    price: high_low
#/  TSLA:
#/    reversal:
#/      type: pct
#/      value: 0.08
#/  NVDA:
#/    reversal:
#/      1D:
#/        type: pct
#/        value: 0.02
#/      5Y:
#/        type: pct
#/        value: 0.10

#/ Apply a custom theme
#/
#/ All colors are optional. If commented out / omitted, the color will get sourced
#/ from your terminal color scheme
#theme:
#/  background: '#403E41'
#/  gray: '#727072'
#/  profit: '#ADD977'
#/  loss: '#FA648A'
#/  text_normal: '#FCFCFA'
#/  text_primary: '#FFDA65'
#/  text_secondary: '#79DBEA'
#/  border_primary: '#FC9766'
#/  border_secondary: '#FCFCFA'
#/  border_axis: '#FC9766'
#/  highlight_focused: '#FC9766'
#/  highlight_unfocused: '#727072'

