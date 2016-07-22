# nerdtree-iterm

## Introduction

iterm\_menu\_item is a [NERDTree](https://github.com/scrooloose/nerdtree)
plugin that adds a menu item to open the selected folder in
[iTerm2](https://iterm2.com/). (i.e. open a shell window and cd to that
folder)

## Installation

### Pathogen

Use the following commands:

    cd ~/.vim/bundle
    git clone https://github.com/mortonfox/nerdtree-iterm.git

### Vundle

Add the following to your vimrc:

    Plugin 'mortonfox/nerdtree-iterm'

Install with ```:PluginInstall```.

### Manual Installation

Copy ```iterm_menu_item.vim``` to ```~/.vim/nerdtree_plugin/``` (*nix)
or ```~/vimfiles/nerdtree_plugin``` (Windows).

### iTerm2 3.x

nerdtree-iterm uses a piece of AppleScript code to open an iTerm session. This
AppleScript code is different for iTerm2 2.x and for iTerm2 3.x.

By default, nerdtree-iterm supports iTerm2 2.x. If you are using iTerm2 3.x (or
an iTerm2 2.9 nightly build), add the following to your vimrc:

    let g:nerdtree_iterm_iterm_version = 3

## Usage

In the NERDTree window, select the desired folder and then type ```m```
and ```i``` to open an iTerm2 session with that folder as the current
directory. If the selection is on a file, this plugin will open iTerm on the
enclosing folder.
