# `vim` - Who needs a mouse?

In this talk, we will use the `neovim` fork of the `vim` editor.
This is a conscious choice because of `neovim`'s portability and OS-neutrality.
The functionality between the two is almost completely the same,
as `neovim` is written to (almost) seamlessly support `vim` configurations.
The configurations shown during the talk will work equally well with the standard version of `vim`.

In order to follow along with the talk, please prepare the following:

## Windows

### Prerequisites

* Python 3.x - [get it here](https://www.python.org/), install it and make sure it's added to your PATH variable
* *Git for Windows* or a comparable implementation of `git`, as we will be cloning some repositories

### Installation

* download the latest version of the [neovim editor](https://github.com/neovim/neovim/releases/tag/v0.4.4)
* extract it to a directory that is easy to access (`C:\tools\neovim` or similar)
* create a directory `nvim` in `C:\Users\<USERNAME>\AppData\Local\`
* in the `nvim` directory, create a file called `init.vim`
* open a command line and run `pip install neovim`

## Linux

### Prerequisites

* Python 3.x - install it with your distro's package manager, check if you have access to the `pip` command on your command line
* Git - install it with your distro's package manager

### Installation

|-----------------------|---------------------------------------------|
| Distro                | Package manager command                     |
|-----------------------|---------------------------------------------|
| *Ubuntu/Debian Linux* | `sudo apt install neovim`                   |
| *Arch Linux*          | `sudo pacman -S neovim`                     |
| *Fedora Linux*        | `sudo dnf install -y neovim python3-neovim` |
|-----------------------|---------------------------------------------|

* create the folder `$HOME/.config/nvim`
* inside the `nvim` folder, create a file called `init.vim`
* in your shell, run the command `pip install neovim`

