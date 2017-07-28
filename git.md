Undo last commit and reflect on index (stagged)
```
    git reset --soft HEAD~
```
Undo last commit and reflect on unstagged
```
    git reset --mixed HEAD~
```
Undo the last commit
```
    git reset --hard HEAD~
```
Reset the current branch to orgin/branch 
```
    git reset --hard origin/branch
```
Remove file from git index (make then untracked)
```
    git rm --cached file
```
Remove untracked files
```
    git clean -f
```
Remove untracked files and directories
```
    git clean -df
```

Add remote to a local repo
```
    git remote add <remote-name> <url>
```
cat .git/config to see the newly added remote.
