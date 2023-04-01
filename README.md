# Kud 
Simple Version Control System to records changes to set of files.
This program can only work on bash shell.

## Requirements
- rsync

## How to Build

- Build program using makefile
```
make
```

- Set permission for executable file and script
```
chmod +x kud
chmod +x src/command/*.sh
```

- Add program to PATH

```
export PATH="$PATH:`pwd`/bin"
```

## How to Run

If program is added to PATH, then run the program using syntax below

```
kud <command>
```


## Available Commands
- `init` - To create repository on pwd
- `commit <commit-msg>` - To add current repository condition to snapshot
- `log` - To see commit history
- `head <version-id>` - To change current directory to version that match
- `tag <version-id> <tag-name>` - To create symbolic link version-id that match on folder `.kud/refs/tags`
