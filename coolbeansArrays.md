#Create exclude list with arrays


I needed a way to store a list in memory.
So, a quick simple way to store your excludes
list within the shell script is to use arrays.




```
list=(
    --exclude *.iso
    --exclude *.tgz
)
```

Then to call it in rsync do:

```
rsync -rtlhuiP --delete-excluded ${list[*]} $source $destination
```