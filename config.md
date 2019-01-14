`git command`
---
Get and set repository or global options.

### synopsis
```vim
git config [<file-option>] [type] [-z|--null] name [value [value_regex]]
git config [<file-option>] [type] --add name value
git config [<file-option>] [type] --replace-all name value [value_regex]
git config [<file-option>] [type] [-z|--null] --get name [value_regex]
git config [<file-option>] [type] [-z|--null] --get-all name [value_regex]
git config [<file-option>] [type] [-z|--null] --get-regexp name_regex [value_regex]
git config [<file-option>] --unset name [value_regex]
git config [<file-option>] --unset-all name [value_regex]
git config [<file-option>] --rename-section old_name new_name
git config [<file-option>] --remove-section name
git config [<file-option>] [-z|--null] -l | --list
git config [<file-option>] --get-color name [default]
git config [<file-option>] --get-colorbool name [stdout-is-tty]
git config [<file-option>] -e | --edit
```

---
### description

You can query/set/replace/unset options with this command. The name is actually the section and the key separated by a dot, and the value will be escaped.

Multiple lines can be added to an option by using the **--add** option. If you want to update or unset an option which can occur on multiple lines, a POSIX regexp value_regex needs to be given. Only the existing values that match the regexp are updated or unset. If you want to handle the lines that do not match the regex, just prepend a single exclamation mark in front (see also the section called "EXAMPLES").

The type specifier can be either **--int** or **--bool**, to make git config ensure that the variable(s) are of the given type and convert the value to the canonical form (simple decimal number for int, a "true" or "false" string for bool), or **--path**, which does some path expansion (see --path below). If no type specifier is passed, no checks or transformations are performed on the value.

The `file-option` can be one of **--system**, **--global** or **--file** which specify where the values will be read from or written to. The default is to assume the config file of the current repository, .git/config unless defined otherwise with GIT_DIR and GIT_CONFIG (see the section called "FILES").

This command will fail if:

1. The config file is invalid,
2. Can not write to the config file,
3. no section was provided,
4. the section or key is invalid,
5. you try to unset an option which does not exist,
6. you try to unset/set an option for which multiple lines match, or
7. you use --global option without $HOME being properly set.

---
### options
> This section is empty yet.

---
### hints
> This section is empty yet.

---
### examples

> git config --global [color.ui auto] [core.autocrlf true] [credential.helper wincred] 

> git config --global user.name "rubber"

> git config --global user.email iarregi86@gmail.com

> git config --global color.ui true