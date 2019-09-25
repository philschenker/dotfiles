# My personal dotfiles

In this repo I store my personal dotfiles. Nothing special I was mostly inspired by LukeSmitzxyz and others. This is thought to be constantly evolving config.

## How to clone

This is taken from Atlassian: https://www.atlassian.com/git/tutorials/dotfiles

Add alias to .bashrc or .zshrc or whatever is used:

```
alias dotgit='/usr/bin/git --git-dir=$HOME/.dotfiles.git --work-tree=$HOME'
```

Adjust .gitignore:

```
echo ".dotfiles.git" >> .gitignore
```

Clone repo:

```
git clone --bare git@github.com:philschenker/dotfiles.git $HOME/.dotfiles.git
```

Check files out:

```
dotgit checkout
```