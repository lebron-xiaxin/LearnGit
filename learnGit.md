> **git log**---查看日志

1. git log --all 查看所有分支的历史
2. git log --all --graph 查看图形化的 log 地址
3. git log --oneline 查看单行的简洁历史。
4. git log --oneline -n4 查看最近的四条简洁历史。
5. git log --oneline --all -n4 --graph 查看所有分支最近 4 条单行的图形化历史。
6. git help --web log 跳转到git log 的帮助文档网页

> **gitk**---通过图形化界面工具查看版本历史

1.gitk

> **git mv**---给文件重命名的简便方法

1.git mv readme new (readme：原文件名。new:新文件名)

> **git-需要做的最小配置**

1. 添加配置：

   git config --local user.name 'XXX'
   git config --local user.email 'XXX@163.com'

2. 参数区别:
   git config --local ##只对某个仓库有效,切换到另外一个仓库失效（本地仓库）
   git config --global ##当前用户的所有仓库有效,工作当中最常用（当前用户的所有仓库）
   git config --sysstem ##系统的所有用户,几乎不用（本系统的所有用户）

3. 查看配置:

   git config --list --local ##只能在仓库里面起作用, 普通路径git不管理
   git config --list --global
   git config --list --system

> 清除设置

1. git config --unset --local user.name
2. git config --unset --global user.name
3. git config --unset --system user.name

> 建立Git仓库

1.把已有项目带入纳入Git管理

cd 项目所在代码文件夹

git init

2.新建项目直接用Git管理

cd 某个文件夹

git init your project #会在当前路劲下创建和项目名称同名的文件夹

cd your project

> git add 提交暂存区

1. git add -u：将文件的修改、文件的删除，添加到暂存区。
2. git add .：将文件的修改，文件的新建，添加到暂存区。
3. git add -A：将文件的修改，文件的删除，文件的新建，添加到暂存区。

git add -A相对于git add -u命令的优点 ： 可以提交所有被删除、被替换、被修改和新增的文件到数据暂存区，而git add -u 只能操作跟踪过的文件，git add -A 等同于git add -all

> git push

1. git push origin master:master      #本地仓库master分支推动到远程仓库的master分支
2. git push origin master　　　　　 #本地仓库当前分支的推送到master分支
3. git push 　　　　　　　　　　　 #将当前本地仓库所在分支提交到远程相同分支下

> 其他命令

1. **清屏**
   Mac: clear
   Windows: clear

2. **展示文件夹内的内容**

   Mac: ls -al
   Windows: dir

3. **展示文件内容（比如展示style.css的内容）**
   Mac: vi style.css
   Windows: more style.css



