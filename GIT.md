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

## fetch
```bash
# After fetching, remove any remote-tracking references that no longer exist on the remote (-p || --prune)
git fetch -p
```
