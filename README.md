# git-gists

### .gitconfig
```
[alias]
    s = status
    lg = !git log --pretty=format:\"%C(magenta)%h%Creset -%C(red)%d%Creset %s %C(dim green)(%cr) [%an]\" --abbrev-commit -15
    br = branch -v --sort=committerdate
    co = checkout
    cob = checkout -b
    res = !git reset --hard
    save = !git add -A && git commit -m 'SAVEPOINT'
    wip = commit -am 'WIP'
    undo = reset HEAD~1 --mixed
    done = !git push origin HEAD
    fe = !git fetch --all
    aliases = !git config --get-regexp 'alias.*' | colrm 1 6 | sed 's/[ ]/ = /' | sort

[core]
    excludesfile = ~/.gitexcludes 
```

### .gitexcludes
```
.DS_Store
.idea
*.iml
```

