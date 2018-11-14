# pyenv-zsh-plugin

[oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh) plugin to set up the pyenv environment

### System Requirements

[pyenv](https://github.com/pyenv/pyenv#basic-github-checkout)

[Build Environment](https://github.com/pyenv/pyenv/wiki#suggested-build-environment)

```shell
sudo apt install -y make build-essential libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev xz-utils tk-dev libxml2-dev libxmlsec1-dev libffi-dev
```

### Installing

Copy the following into your zsh shell.

```shell
git clone https://github.com/philjc/pyenv-zsh-plugin.git "$ZSH_CUSTOM/plugins/pyenv-pjc"

# Automatically open .zshrc with vim with the search and replace string to activate the pyenv plugin
# just hit 'y' and then ':wq' to save
vim -c ":%s/^plugins=(/plugins=(\r  pyenv-pjc/gc" $HOME/.zshrc && source $HOME/.zshrc
```
