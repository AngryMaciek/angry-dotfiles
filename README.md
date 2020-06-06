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
cd $HOME && git clone https://github.com/AngryMaciek/small-dotfiles.git
```

## Stow the dotfiles

**Remember to backup all your current config files before the linking**  

Use `stow` to create proper symlinks:
```bash
stow -vSt ~ small-dotfiles/dotfiles/git
stow -vSt ~ small-dotfiles/dotfiles/pylint
stow -vSt ~/.config/htop small-dotfiles/dotfiles/htop
```

## License

Unlicense

---
Missing:
* tmux
* guake
