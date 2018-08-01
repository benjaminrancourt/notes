# Bash
## Cheatsheet
* **[devhints.io](https://devhints.io/bash)**

## Iterate over directories
```bash
#!/bin/bash
echo "Bash version ${BASH_VERSION}..."
for directory in $(ls -d */ | cut -f1 -d'/')
do
    cd $directory/trunk
    pwd
done
```
