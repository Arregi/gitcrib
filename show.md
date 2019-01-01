`git show`
---
Show various types of objects.

### synopsis
```vim
[options] <object>…​
```
---
### options
> `[commit_ID]` Shows the differences introduced by a commit compared to its parent.
---
### hints

> For commits it shows the log message and textual diff. It also presents the merge commit in a special format as produced by git diff-tree --cc.

> For tags, it shows the tag message and the referenced objects.

> For trees, it shows the names (equivalent to git ls-tree with --name-only).

> For plain blobs, it shows the plain contents.

> The command takes options applicable to the git diff-tree command to control how the changes the commit introduces are shown.

---
### examples

>  git show [commit_ID]

