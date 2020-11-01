# `vim` - Tutorial

The following is a tutorial to install the `pathogen.vim` plugin manager and the `UltiSnips` snippet manager plugin.

## Install the `pathogen.vim` Plugin Manager

* In your `nvim` configuration folder, create directories `autoload` and `bundle`.
* Download the pathogen plugin file at `http://tpo.pe/pathogen.vim` and place it into your `autoload` folder.

## Add `pathogen` to your `init.vim`

* In your `init.vim`, add the following lines:

```
execute pathogen#infect()
call pathogen#helptags()
syntax on
filetype plugin indent on
```

## Install the `UltiSnips` Plugin

* Initialize a git repository in your `nvim` folder by running `git init`.
* Clone the `UltiSnips` repository in your `bundle` directory by calling

```
git submodule add https://github.com/sirver/ultisnips
```

## Configure the `UltiSnips` Plugin

* Create a folder called `mysnips` (or similar) in your `nvim` folder.
* In your `init.vim`, after the `pathogen` call, add the following:

```
let g:UltiSnipsSnippetDirectories['/path/to/mysnips']
let g:UltiSnipsExpandTrigger="<tab>"
let g:UltiSnipsJumpForwardTrigger="<c-j>"
let g:UltiSnipsJumpBackwardTrigger="<c-k>"
```
## Create a new Java Snippet File

* Create a new Java class file somewhere in your file system.
* Open the new Java class with Neovim.
* Type `:UltiSnipsEdit` to open a new Java snippet file.
* Create your snippets!

