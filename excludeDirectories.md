Excluding directories with --exclude

```
# Excludes list
list=(
          --exclude 'Crash*Reports/'
          --exclude *.iso
)
```

To exclude a directory that contain spaces the only way that I've found that works is to use an asterisk in replace of the space. Neither a slash-space (\ ) nor a period (.) worked.

I'm using RSYNC version 3.0.9 protocol version 30, the one that came with cygwin.