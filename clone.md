git clone <repository>
---
Clone a repository into a new directory.
        
### synopsis

```vim
 [--template=<template_directory>]
 [-l] [-s] [--no-hardlinks] [-q] [-n] [--bare] [--mirror]
 [-o <name>] [-b <name>] [-u <upload-pack>] [--reference <repository>]
 [--dissociate] [--separate-git-dir <git dir>]
 [--depth <depth>] [--[no-]single-branch] [--no-tags]
 [--recurse-submodules[=<pathspec>]] [--[no-]shallow-submodules]
 [--jobs <n>] [--] <repository> [<directory>]
```

---
### hints
> Makes a clone of the whole repository, all the files and the whole history of branches and commits.

> You must specify a repository to clone.
---
### examples

> git clone https://github.com/arregit/gitcrib.git