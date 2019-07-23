# `git --help` Help Document

```shell
usage: git [--version]
           [--help]
           [-C <path>]
           [-c name=value]
           [--exec-path[=<path>]]
           [--html-path]
           [--man-path]
           [--info-path]
           [-p | --paginate | --no-pager]
           [--no-replace-objects]
           [--bare]
           [--git-dir=<path>]
           [--work-tree=<path>]
           [--namespace=<name>]
           <command> [<args>]
```
**Others Languages:** [Chinese](./GitHelpCN.md)

<!-- vim-markdown-toc GFM -->
- [`git --help` Help Document](#git---help-help-document)
  - [These are common Git commands used in various situations:](#these-are-common-git-commands-used-in-various-situations)
      - [1.start a working area (see also: `git help tutorial`)](#1start-a-working-area-see-also-git-help-tutorial)
      - [2.work on the current change (see also: `git help everyday`)](#2work-on-the-current-change-see-also-git-help-everyday)
      - [3.examine the history and state (see also: `git help revisions`)](#3examine-the-history-and-state-see-also-git-help-revisions)
      - [4.grow, mark and tweak your common history](#4grow-mark-and-tweak-your-common-history)
      - [5.collaborate (see also: `git help workflows`)](#5collaborate-see-also-git-help-workflows)
<!-- vim-markdown-toc -->

## These are common Git commands used in various situations:

#### 1.start a working area (see also: `git help tutorial`)
| SubCommend | Resume
|:----------:|-------
| `clone`    | Clone a repository into a new directory  
| `init`     | Create an empty Git repository or reinitialize an existing one

#### 2.work on the current change (see also: `git help everyday`)
| SubCommend | Resume
|:----------:|-------
| `add`      | Add file contents to the index
| `mv`       | Move or rename a file, a directory, or a symlink
| `reset`    | Reset current HEAD to the specified state
| `rm`       | Remove files from the working tree and from the index

#### 3.examine the history and state (see also: `git help revisions`)
| SubCommend | Resume
|:----------:|-------
| `bisect`   | Use binary search to find the commit that introduced a bug
| `grep`     | Print lines matching a pattern
| `log`      | Show commit logs
| `show`     | Show various types of objects
| `status`   | Show the working tree status

#### 4.grow, mark and tweak your common history
| SubCommend | Resume
|:----------:|-------
| `branch`   | List, create, or delete branches
| `checkout` | Switch branches or restore working tree files
| `commit`   | Record changes to the repository
| `diff`     | Show changes between commits, commit and working tree, etc
| `merge`    | Join two or more development histories together
| `rebase`   | Reapply commits on top of another base tip
| `tag`      | Create, list, delete or verify a tag object signed with GPG

#### 5.collaborate (see also: `git help workflows`)
| SubCommend | Resume
|:----------:|-------
| `fetch` | Download objects and refs from another repository
| `pull` | Fetch from and integrate with another repository or a local branch
| `push` | Update remote refs along with associated objects

> '`git help -a`' and '`git help -g`' list available subcommands and some concept guides.  
> See '`git help <command>`' or '`git help <concept>`' to read about a specific subcommand or concept.
