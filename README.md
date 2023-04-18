# Homebrew

## Formulas

- nvm
- zsh
- node
- yarn
- git-remote-codecommit
- visual-studio-code
- cfn-lint
- yarn

# Zsh

## Installation

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
zsh --version
upgrade_oh_my_zsh
```

## Plugins

#### zsh-autosuggestions

`git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`

### Fuzzy file finding (FZF )
FZF is a fuzzy file finder that enables you to search for files interactively from the command line. It is really useful for quickly finding files when you know the name but can’t remember exactly where you saved it.

# install FZF (say yes to each option during installation)
git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf
~/.fzf/install
The installation script will automatically update your .zshrc with the following line:

[ -f ~/.fzf.zsh ] && source ~/.fzf.zsh
Additionally, to get fzf to play nice with oh-my-zsh you will need to add fzf to your list of plugins and set an environment variable with the fzf installation location:

# update your ~/.zshrc file
FZF_BASE="$HOME/.fzf"

plugins=(
    zsh-syntax-highlighting 
    zsh-autosuggestions
    fzf
)
You can now activate the fuzzy finder by either typing fzf as a command to your terminal or pressing CTRL+T. You can also trigger the fuzzy finder using the ** prefix and pressing <TAB> (see documentation ). For example:

# search which file to open in vim using the fuzzy finder
vim **<TAB>
FZF is highly customisable. I won’t go into too much detail here on how to configure it – it probably requires an entire blog post in itself. But there are plenty of great tutorials online explaining how to configure FZF which I recommend you investigate to get the most out of it.

## Colors

[profile](default.json)

## Font

[Meslo Powerline](https://github.com/powerline/fonts/blob/master/Meslo%20Dotted/Meslo%20LG%20S%20DZ%20Regular%20for%20Powerline.ttf)

# VsCode

[profile](profile.code-profile)
