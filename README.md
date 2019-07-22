# VSCodeWithProgram
@[TOC](文章目录)
## 1.Git command line simple operation
> [Git-简明指南](http://rogerdudler.github.io/git-guide/index.zh.html )

* 创建新仓库 `git init`
* 克隆已有仓库 `git clone`
```shell
# 本地仓库路径
git clone /path/to/repository
# 远程仓库路径
git clone username@host:/path/to/repository
# .EXAMPLE
git clone https://github.com/empyrealtear/VSCodeWithProgram.git
```
* 工作流(提交修改的文件)
> 添加文件至暂存区 **Index**. `git add <filename>`  
> 添加提交信息至 **HEAD**. `git commit -m "代码提交信息"`  
> 推送文件至分支 `git push origin master`  
> Note: `master` 为默认主分支, 可将其替换为要推送到的分支
