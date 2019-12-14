### git工具使用



#### Git 的基本命令操作

1.  git innt // 初始化本地git仓库
2. git add <file> // 添加文件
3. git status // 查看状态
4. git commit //提交
5. git push  //推送到仓库
6. git pull   //从远程仓库拉取数据
7. git clone //从远程仓库拷贝数据

##### 忽略文件

​	.gitignore

### 增

 add

 1. 添加指定文件或目录到本地暂存区  // git add 'file'或'dir'

 2. 添加目录下所有文件到本地暂存区 // git add *

    ### 删 rm

    1. 从git 代码库中移除文件  //git rm 'file'
    2. 从git 代码库中移除目录 // git rm r 'dir'

    ### 改 ： commit

    1. 提交暂存区内容到git代码仓库 //git commit -m 'commit message'
    2. 提交暂存区指定文件到git代码仓库 // git commit 'file' -m 'commit message'
    3. 提交工作区内容到git仓库 （不需要git add） //git commit -a
    4. 提交一次新信息替换上一次提交 （如果没有发生变化，改写上一次提交信息）// git commit --amend -m 'message'

    

### 查

1. 显示有更变的文件 

   * git status

   2.显示暂存区和工作区的区别

   * git diff 

   3.显示当前分支的历史版本信息

   * git log 

   4.根据关键搜索提交历史信息

   * git log -s 'keycode'

   5.显示指定文件修改详情

   * git blame 'file'

   6.显示当前分支的最近几次提交

   * git reflog

### 分支 ： branch

1.列出所有本地分支

* git branch

2. 列出所有远程分支
   * git branch -r 

3. 列出所有本地远程分支

   * git branch -a

   4.新建一个分支 ， 但保持在当前分支

   * git branch 'branch name'

   5.删除分支

   * git branch -d 'branch name'

### 检验： checkout

  1. 恢复暂存区的文件到工作区

     * git checkout 'file'

     2.恢复暂存区的所有文件到工作区

     * git checkout *

     3.切换到上一个分支

     * git checkout 

     4.新建一个分支，并切换到该分支

     * git checkout -b 'branch name'

### 合并 ：merge

1. 将分支合并到当前分支
   * git merge "barnch name"

### 远程： remote

 1.显示所有远程git代码库

* git remote -v
  2. 显示指定远程git 代码库信息
     * git remote show 'remote name'

### 推送： push

 1. 提交标签到指定远程git代码仓库

    * git push 'remote name ' "tag name"

    2.提交分支到指定远程git 代码库

    * git push 'remote name' 'branch name'

    3.强行提交当前分支到远程代码库

    * git push 'remote name' -force(分支名)