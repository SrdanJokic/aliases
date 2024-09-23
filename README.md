# aliases
Aliases and faster commands for doing things

# Git

```
git config --global alias.nccommit 'commit --allow-empty-message -m ""' && git alias glog="git log --oneline --graph --all --decorate" && git alias gb="git branch -vv" && git config --global alias.alias "! git config --get-regexp ^alias\. | sed -e s/^alias\.// -e s/\ /\ =\ /"
```
