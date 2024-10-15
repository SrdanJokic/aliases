# aliases
Aliases and faster commands for doing things

# Git

The command:
```
git config --global alias.nccommit 'commit --allow-empty-message -m ""' && git config --global alias.glog 'log --oneline --graph --all --decorate' && git config --global alias.gb 'branch -vv' && git config --global alias.checkpoint '!git add . && git nccommit && git push -u origin HEAD' && git config --global alias.alias "! git config --get-regexp ^alias\. | sed -e s/^alias\.// -e s/\ /\ =\ /"
```

... results in `~/.gitconfig`:

Elementary commands:
```
nccommit = commit --allow-empty-message -m \"\"  # commit with no message
glog = log --oneline --graph --all --decorate  # log nicely
gb = branch -vv  # print the branch and the last commit in one line
```

Composite commands:
```
checkpoint = '!git add . && git nccommit && git push -u origin HEAD'  ## adds an empty commit and pushes to remote
alias = '!git config --get-regexp ^alias\\. | sed -e s/^alias\\.// -e s/\\ /\\ =\\ /'  # list aliases
```
