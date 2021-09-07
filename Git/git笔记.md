Git使用的命令和linux一样，因为他们是一个公司生产的产品。你可以尽情的使用Linux命令，去操作Git。

# 查看版本

git --version

# 设置用户名

git config --global user.name 用户名

# 设置邮箱 

 git config --global user.email 邮箱名

邮箱的虚拟的，可以随便设置，注意格式就行。

# 查看git设置的配置文件

cat ~/.gitconfig 

# 添加文本

vim <file> 	

点击i键，进行编辑，使用esc退出编辑，输出wq!保存退出。

# 查看状态

git status

# 添加暂存区

git add <file> 

再次查看的状态的时候，提交到暂存区的文件变成了绿色的字体了，说明此文件暂存区有一份，本地工作区有一份，删除文件只是删除暂存区，本地的文件依然存在。

# 删除暂存区的文件

git rm -cached <file>

# 提交

git commit -m "first commit" hello.txt 第四个参数是每次提交的次数，我这里是第一次提交，查看状态 On branch master nothing to commit, working tree clean 文件中没有修改内容，所以工作树干净，不用提交。

# 查看版本信息

git reflog

# 查看版本详细信息

git log

# 版本穿梭

![img](.\clipboard.png)

git reset --hard 版本号 head指针指向master，master根据的自己修改的文件内容信息，去指定版本。(移动的是master的指针，其他不动)

# 查看分支

git branch -v

# 添加分支

git branch 分支名

# 指向分支

git checkout 分支名

# 合并分支

git merge 分支名

