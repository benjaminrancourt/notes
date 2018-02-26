# SVN
## log
```bash
# Print out the last tag.
svn log -v $SVN/path/tags --limit 1 | awk '/^   A/ { print $2 }' | grep -v RC |  head -1
# /path/tags/1.0.1
```
