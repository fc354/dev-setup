# dev-setup
Development environment setup on MAC

## Homebrew
`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"`

## OMZ
Install oh-my-zsh: https://ohmyz.sh/#install

`sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

Add autosuggestions: https://github.com/zsh-users/zsh-autosuggestions

`git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`

Add the plugin to the list of plugins for Oh My Zsh to load (inside ~/.zshrc):

`plugins=( 
    # other plugins...
    zsh-autosuggestions
)`
note plugins are separated by space not comma

## Tmux 
Tmux may be good enough out of the box, but can be more powerful tho. Here is a useful video: https://youtu.be/DzNmUNvnB04

Get the TPM first: https://github.com/tmux-plugins/tpm

If I may only suggest one plugin, I say add the mouse support

`set -g mouse on`

## Python
`brew install python`

remeber to create/ manage your venv

`python -m venv venv`

## Notebook extensions
https://github.com/ipython-contrib/jupyter_contrib_nbextensions

Install the extensions
`pip install jupyter_contrib_nbextensions`

Install non-python requirements
`jupyter contrib nbextension install --user`

Install the configurator
`pip install jupyter_nbextensions_configurator`

