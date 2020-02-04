# Bash
## Links
* [Linux Bash->SED compatible online escape character tool](http://dwaves.de/tools/escape/)
* **[devhints.io](https://devhints.io/bash)** - Cheatsheet

## Count the number of lines for files
```bash
find -name '*.js' | xargs wc -l
```

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
