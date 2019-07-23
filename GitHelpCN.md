**其他语言:** [英文版](./GitHelpEN.md)

<!-- vim-markdown-toc GFM -->
- [`git --help` 帮助文档](#git---help-帮助文档)
  - [一些在各种情况下使用的Git常见命令](#一些在各种情况下使用的Git常见命令)
    - [1.启用一个工作空间](#1启用一个工作空间-更多参阅-git-help-tutorial)
    - [2.处理当前更改](#2处理当前更改-更多参阅-git-help-everyday)
    - [3.检查历史和状态](#3检查历史和状态-更多参阅-git-help-revisions)
    - [4.添加、标记和调整你的共同历史](#4添加、标记和调整你的共同历史)
    - [5.协作](#5协作-更多参阅-git-help-workflows)
<!-- vim-markdown-toc -->

# `git --help` 帮助文档

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


## 一些在各种情况下使用的Git常见命令:

#### 1.启用一个工作空间 (更多参阅: `git help tutorial`)
|   子命令   | 简述
|:----------:|-----
| `clone`    | 克隆一个存储库到新存储库中
| `init`     | 创建一个空Git存储库或重新初始化现有的存储库

#### 2.处理当前更改 (更多参阅: `git help everyday`)
|   子命令   | 简述
|:----------:|-----
| `add`      | 将文件内容添加到暂存区(**Index**)
| `mv`       | 移动或重命名文件, 目录或符号链接
| `reset`    | 将当前**HEAD**重置为指定状态
| `rm`       | 从 working tree 和暂存区(**Index**)中移除文件

#### 3.检查历史和状态 (更多参阅: `git help revisions`)
|   子命令   | 简述
|:----------:|-----
| `bisect`   | 使用二进制搜索查找引入错误的提交
| `grep`     | 打印与图案匹配的线条
| `log`      | 显示提交日志
| `show`     | 显示各种类型的对象
| `status`   | 显示 working tree 状态

#### 4.添加、标记和调整你的共同历史
|   子命令   | 简述
|:----------:|-----
| `branch`   | 列出、创建或删除分支
| `checkout` | 切换分支或还原工作树文件
| `commit`   | 记录对存储库的更改
| `diff`     | 显示 commits、commit 和 working tree 等之间的更改
| `merge`    | 将两个或多个开发历史连接在一起
| `rebase`   | 在另一个基本提示上重新应用提交
| `tag`      | 创建、列出、删除或验证用 GPG 签名的标记对象

#### 5.协作 (更多参阅: `git help workflows`)
|   子命令   | 简述
|:----------:|-----
| `fetch`    | 从另一个存储库下载对象和引用
| `pull`     | 从另一个存储库或本地分支获取并与之集成
| `push`     | 更新远程引用和关联对象

> '`git help -a`' 与 '`git help -g`' 列出可用的子命令和一些概念指南。  
> 参阅 '`git help <command>`' or '`git help <concept>`' 以了解特定的子命令或概念。