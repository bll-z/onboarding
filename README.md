# onboarding
install your new computer

## xcode

    # Update xcode
    xcode-select --install

## brew

    ## Install Brew (apt-get for osx)
    ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)
    ## cask (Application installation through brew)
    brew tap caskroom/cask
    brew  install caskroom/cask/brew-cask
    ## and versions (install older versions of packages with brew)
    brew tap caskroom/versions
    
    ## maintenance
    brew doctor # will diagnose potential problems
    brew update
    brew cask update
    
    ## Optionally install some of your tools with brew
    brew install [wget, git, vim, python, python3, ruby, node, npm, docker]
    brew cask install [google-chrome, virtualbox, theunarchiver, balsalmiq, sourcetree, sublime-text3]

## dotfiles
Files that you can quickly clone to your home directory that establish many of the settings of your computer

* Brewfile - you can keep a list of your brew and cask installed dependencies to quickly reinstall all the same packages
* bash files 
  * startup files - http://www.gnu.org/software/bash/manual/html_node/Bash-Startup-Files.html#Bash-Startup-Files
  * bash prompt basics - http://linuxconfig.org/bash-prompt-basics
* vim settings (ie .vimrc) - google it the possibilities are endless
* git settings (.gitignore, .gitconfig, etc.)
* .inputrc - settings for your terminal input (eg changing tab complete behavior)
* google dotfiles for more info

## editing your path
The path is the setting that tells your terminal what order to check directories for commands you try to run
For instance all of your brew commands live in /usr/local/bin
In one of your files that is run whent he terminal
is opened, you update your path with the following syntax

    # prepend to path
    export PATH="/path/to/commands:$PATH"
    # append to path
    export PATH="$PATH:/path/to/commands"

## Conclusion
Congratulations, you are now ready to clone a project and get going.




