# .FILES
*Maciek Bak*  

My personal configuration schemes for various software.  
(Dedicated to Linux systems)

## Install Git and Stow

[Git](https://git-scm.com/) is an open source version control system. In principle one can download this repository manually, as a compressed package, but I highly recommend to install `git` first and then use it to pull all the files automatically.  

[GNU Stow](https://www.gnu.org/software/stow/) is a symbolic link manager, particularly useful for setting up configuration files. In principle one could move the files into their proper location by hand, but again - why bother with manual labour while there are dedicated tools that will do the job for you? :wink:

Please execute:
```bash
sudo apt-get install git stow --yes
```

## Clone the repository

Use `git` command to clone this repository into your local machine:
```bash
git clone https://github.com/AngryMaciek/small-dotfiles.git
```

## Stow the dotfiles

Use `stow` to create proper symlinks:
```bash
stow -vSt ~ git pylint
```

---
Missing:
* tmux
* terminator
* vscode? (https://pawelgrzybek.com/sync-vscode-settings-and-snippets-via-dotfiles-on-github/)
* iterm2
* guake
* htop