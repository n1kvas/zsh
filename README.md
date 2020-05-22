# zsh
My ZSH Config

## Setup
```
wget https://github.com/n1kvas/zsh/raw/master/.zshrc -O ~/.zshrc
mkdir -p "$HOME/.zsh"
wget https://github.com/n1kvas/zsh/raw/master/.zsh/aliasrc -O ~/.zsh/aliasrc
git clone https://github.com/sindresorhus/pure.git "$HOME/.zsh/pure"
```
## Get Dependancies 
  - zsh-syntax-highlighting - syntax highlighting for ZSH in standard repos
  - autojump - jump to directories with j or jc for child or jo to open in file manager
  - zsh-autosuggestions - Suggestions based on your history
  
Finish the conversion by changing your user in /etc/passwd to /bin/zsh instead of /bin/bash

## Install

1. There are two main ways to install Zsh
  - with the package manager of your choice, _e.g._ `sudo apt install zsh` (see [below for more examples](#how-to-install-zsh-in-many-platforms))
  - from [source](http://zsh.sourceforge.net/Arc/source.html), following
        [instructions from the Zsh FAQ](http://zsh.sourceforge.net/FAQ/zshfaq01.html#l7)
2. Verify installation by running `zsh --version`. Expected result: `zsh 5.4.2` or more recent.
3. Make it your default shell: `chsh -s $(which zsh)`
  - Note that this will not work if Zsh is not in your authorized shells list (`/etc/shells`)
    or if you don't have permission to use `chsh`. If that's the case [you'll need to use a different procedure](https://www.google.com/search?q=zsh+default+without+chsh).
    #Debian
    sudo su
    chsh -s /usr/bin/zsh root 
    
4. Log out and login back again to use your new default shell.
5. Test that it worked with `echo $SHELL`. Expected result: `/bin/zsh` or similar.
6. Test with `$SHELL --version`. Expected result: 'zsh 5.4.2' or similar
