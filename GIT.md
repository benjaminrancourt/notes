# Git
## branch
```bash
# List both remote-tracking branches and local branches (-a || --all)
# with sha1 and commit subject line for each head (-v || -vv || --verborse)
git branch -av

# List branches that are already merged in the current branch (ex. master)
git checkout master
git branch --merged
git branch -d old-merged-feature

# List branches that are not merged in the current branch (ex. master)
git checkout master
git branch --no-merged
git branch -D old-abandoned-feature
```

## config
```bash
# Check your settings
git config --list

# Set your identity
git config --global user.name "Benjamin Rancourt"
git config --global user.email benjamin.rancourt@email.com

# Set Vim as default editor for Git
git config --global core.editor vim

# Set some useful aliases (https://git-scm.com/book/tr/v2/Git-Basics-Git-Aliases)
git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.ci commit
git config --global alias.st status

## Unstage a file (git unstage fileA)
git config --global alias.unstage 'reset HEAD --'

## See the last commit easily (git last)
git config --global alias.last 'log -1 HEAD'
```

## fetch
```bash
# After fetching, remove any remote-tracking references that no longer exist on the remote (-p || --prune)
git fetch -p
```
