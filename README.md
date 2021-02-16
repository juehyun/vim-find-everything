# vim-find-everything

This repo folk from 'voldikss/vim-find-everything'

Check original repository for usage and detailed configurations

# Changes

Some characters are not represented properly when use with cp949 window 10 environment.

# Installation

- Install "Everything" from voidtool

	- Install both GUI version (Everything.exe) and command-line tool (es.exe)

- Change gvim guifont setting with which has extended character set (e.g. D2Coding font from naver.com)

	```
	$ edit ~/.vimrc

	set guifont=D2Coding:h13
	```

- Change cmd.exe default codepage to UTF-8

	```
	$ run 'regedit'

	find '컴퓨터\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Command Processor'

	add variable 'Autorun'  (Create the variable as string type if not exist)

	set vaule to 'chcp 65001'
	```

- Add plugin to .vimrc (vim-plug)

	```
	call plug#begin('~/.vim/plugged')
	...
	Plug 'juehyun/vim-find-everything'
	...
	call plug#end()
	```

- Execute ":PlugInstall" at gvim command-line

- Execute ":FE pattern<CR>"


