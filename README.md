# dragvisuals.vim

This is an exact copy of Damian Conway's [dragvisuals.vim](https://github.com/thoughtstream/Damian-Conway-s-Vim-Setup/blob/master/plugin/dragvisuals.vim). I am storing it in my own repo so that I can manage its installation with [Vundle](https://github.com/VundleVim/Vundle.vim).

### Usage

The following installation instructions been modified to use Vundle's directory sturcture for plugins.

Add the following (uncommented) to your .vimrc...

	" Key mappings for dragvisuals.vim

	runtime bundle/dragvisuals/plugins/dragvisuals.vim

	vmap  <expr>  <LEFT>   DVB_Drag('left')
	vmap  <expr>  <RIGHT>  DVB_Drag('right')
	vmap  <expr>  <DOWN>   DVB_Drag('down')
	vmap  <expr>  <UP>     DVB_Drag('up')
	vmap  <expr>  D        DVB_Duplicate()

	" Remove any introduced trailing whitespace after moving...
	let g:DVB_TrimWS = 1
