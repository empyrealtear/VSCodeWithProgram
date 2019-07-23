<!-- vim-markdown-toc GFM -->
- [Git 命令行的一些简单操作](#Git-命令行的一些简单操作)
  - [**一、创建新仓库-Init**](#一、创建新仓库-Init)
  - [**二、克隆已有仓库-Clone**](#二、克隆已有仓库-Clone)
  - [**三、工作流-Add-Commit-Push**](#三、工作流-Add-Commit-Push)
  - [**四、分支-Checkout-Branch-Push**](#四、分支-Checkout-Branch-Push)
  - [**五、更新与合并-Pull-Branch-Diff**](#五、更新与合并-Pull-Branch-Diff)
  - [**六、标签-Tag-Log**](#六、标签-Tag-Log)
  - [**七、日志-Log**](#七、日志-Log)
  - [**八、替换本地内容-Checkout-Fetch-Reset**](#八、替换本地内容-Checkout-Fetch-Reset)
  - [**九、图形化Git**](#九、图形化Git)
<!-- vim-markdown-toc -->

## **Git 命令行的一些简单操作**
> [Git-简明指南](http://rogerdudler.github.io/git-guide/index.zh.html )
> [GitHelpCN.md](./GitHelpCN.md)

### **一、创建新仓库-Init**
| Command | Resume
|:--------|:------
| `git init`                  | 将当前目录作为新存储库
| `git init /path/filefolder` | 将指定文件夹作为新存储库

### **二、克隆已有仓库-Clone**
| Command | Resume
|:--------|:------
| `git clone /path/to/repository`               | 从本地仓库路径克隆
| `git clone username@host:/path/to/repository` | 从远程仓库路径克隆
**Note:** `git clone https://github.com/empyrealtear/VSCodeWithProgram.git`

### **三、工作流-Add-Commit-Push**
| Command | Resume
|:--------|:------
| `git add <filename>`          | 添加文件至暂存区 **Index**
| `git commit -m "代码提交信息"` | 添加提交信息至 **HEAD** 
| `git push origin master`      | 推送改动到远程默认分支
**Note:** `master` 为默认主分支, 可替换为指定分支

### **四、分支-Checkout-Branch-Push**
| Command | Resume
|:--------|:------
| `git checkout -b feature_x` | 创建一个名为 feature_x 的分支, 并切换过去
| `git checkout master`       | 切换回主分支
| `git branch -d feature_x`   | 删除名为 feature_x 的分支
| `git push origin <branch>`  | 推送指定分支到远程仓库

### **五、更新与合并-Pull-Branch-Diff**
| Command | Resume
|:--------|:------
| `git pull` | 更新本地仓库至最新改动
| `git master <branch>` | 合并其他分支到指定分支, 以 `master` 为例
| `git diff <source_branch> <target_branch>` | 合并改动之前, 查看源分支与指定分支的差异
**Note:** 当出现冲突 `confilcts` 时, 做好指定修改后, `git add <filename>` 添加指定文件以使其标记为合并成功
**Note:** 有待实验

### **六、标签-Tag-Log**
* `git tag 1.0.0 1b2e1d63ff`
* 上述命令标记 **Version:** `1.0.0`, **ID:** `1b2e1d63ff`
* `git log` 以查看提交过的 **ID**

### **七、日志-Log**
| Command | Resume
|:--------|:------
| `git log`                  | 查看本地仓库历史日志
| `git log --author=bob`     | 该仓库指定作者的提交日志
| `git log --pretty=oneline` | 压缩显示历史日志至一行
| `git log --graph`          | ASCII 艺术的树形结构来展示所有的分支
| `git log --name-status`    | 查看仓库文件的更改状态
| `git log --help`           | 更多日志命令的子选项

### **八、替换本地内容-Checkout-Fetch-Reset**
| Command | Resume
|:--------|:------
| `git checkout -- <filename>`     | 使用 HEAD 中的最新内容替换掉你的工作目录中的文件
| `git fetch origin`               | 丢弃在本地的所有改动与提交
| `git reset --hard origin/master` | 可以到服务器上获取最新的版本历史，并将你本地主分支指向它
**Note:** 有待实验

### **九、图形化Git**
| Command | Resume
|:--------|:------
| gitk | 内建的图形化 git
| git config color.ui true | 设置为彩色的 git 输出
| git config format.pretty oneline | 显示历史记录时，每个提交的信息只显示一行
| git add -i | 交互式添加文件到暂存区
**Note:** 有待实验