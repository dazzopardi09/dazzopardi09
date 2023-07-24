here's my script for installing everything on my computer:

 #!/usr/bin/env bash

 
 # install brew

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

brew update && brew upgrade

brew installbash-completion

brew install cask

 
# install git

brew install git

 
# install fasd

brew install fasd

 

brew install rsync

brew install wget

brew install tree

brew install fd

 

# install node and yarn

brew install node

brew install yarn

brew install pnpm

 

# install nvm

brew install nvm

mkdir -pv ~/.nvm

echo "export NVM_DIR=\"$HOME/.nvm\"" ~/.bash_profile

echo "[ -s \"$NVM_DIR/nvm.sh\" ] && \. \"$NVM_DIR/nvm.sh\"  # This loads nvm" ~/.bash_profile

echo "[ -s \"$NVM_DIR/bash_completion\" ] && \. \"$NVM_DIR/bash_completion\"  # This loads nvm bash_completion" ~/.bash_profile

echo "source $(brew --prefix nvm)/nvm.sh" ~/.bash_profile

 

# install python

brew install pyenv

 

# install database

brew install sqlite

brew install mysql-client

brew install --cask mysqlworkbench

 

# install ides

brew install --cask atom

brew install --cask jetbrains-toolbox

brew install --cask sublime-merge

brew install --cask sublime-text

brew install --cask visual-studio-code

 

# browsers

brew install --cask brave-browser

brew install --cask chromium

brew install --cask google-chrome

brew install --cask google-chrome-canary

brew install --cask google-chrome-dev

brew install --cask microsoft-edge

brew install --cask firefox

brew install --cask opera

brew install --cask opera-gx

brew install --cask vivaldi

brew install --cask sizzy

 

# terminals

brew install --cask hyper

brew install --cask tabby

 

# tools

brew install --cask postman

brew install --cask rectangle

 

# other stuff

brew install --cask microsoft-teams

brew install --cask microsoft-outlook

brew install --cask figma

brew install --cask zeplin

 

# devops

brew install --cask virtualbox
