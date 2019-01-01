`git log`
---
Show commit logs.

### synopsis
```vim
[<options>] [<revision range>] [[\--] <path>…​]
```
---
### options 

* This section needs some workç

> `[--stat]` Shows some statistics about changes commited.
> `[--oneline]` This is a shorthand for "--pretty=oneline --abbrev-commit" used together. 
> `[--graph]` Draws a text-based graphical representation of the commit history on the left hand side of the output.
> `[-nM]` Shows M commits, starting from the latest one. (M is a number). 
> `[branch_name] [branch_name2]` Shows only commits that belong to this branches.


---
### hints

> Type `q` to exit the log view, and navigate the log with up/down arrows.
---
### examples

> git log --graph --oneline master branch1
