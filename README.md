# dotfiles

This repository contains my dotfiles. I use [GNU Stow](https://www.gnu.org/software/stow/) to manage them.

## Installation

first clone the repository.

```bash
git clone --recursive git@github.com:ZionCorbanie/.dotfiles.git
```

For zsh first download [oh-my-zsh](https://ohmyz.sh/) and remove the default `.zshrc` file.

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
rm ~/.zshrc
```

Then use stow to install the dotfiles.

```bash
cd ~/.dotfiles
stow -t ~ */
```
