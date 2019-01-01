`git diff`
---
Show changes between commits, commit and working tree, etc. (Returns nothing if there is no differences).

### synopsis
```vim
[options] [<commit>] [--] [<path>…​]
```
---
### options
> `[commit_ID1]` Shows **all** the changes performed to that point in the repository.
> `[commit_ID1] [commit_ID2]`  Shows the differences between `commit_ID1` and `commit_ID2` , in the repository. (`commit_ID1` should be the older one, for clarity).
> `--staged` Shows the differences between the staged area and the latest commit of the repository.
---
### hints

> Used without arguments or options, shows the differences between the working tree and the staging area.
---
### examples

> git diff 1a15 96a6	

