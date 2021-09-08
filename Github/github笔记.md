# 远程仓库地址

https://github.com/literaryGiantChen/demo1.git

仓库分支名建议和本地操作的文件夹名一直

# 查看远程仓库别名

git remote -v

# 创建远程仓库别名

 git remote add 别名 远程仓库地址

案列：git remote add demo1 https://github.com/literaryGiantChen/demo1.git

​	别名建议和当前文件名一直

# 推送

git push 远程仓库地址(远程仓库地址别名 或者 远程仓库地址) 分支名

案列：git push demo1 master

# 拉取

git pull 远程仓库地址 分支名

案列：git pull demo1 master



# 克隆远程仓库g本地

git clone 远程仓库地址

案列  git clone git@github.com:literaryGiantChen/demo1.git master



# SSH免密登录

先进入C:\Users\用户名，找到.ssh，删除。没有右键启动git工具

运行命令生成.shh 秘钥目录[参数 -c 一定要是大写的 -C ]

shh-keygen -t rsa -C 远程仓库账号

命令输出完后回车，提示的内容就回车三下

![2021-09-08_102914](D:.\2021-09-08_102914.jpg)

将上面的后缀为pub的格式，所在的路径，复制

输入 cat 地址，将文本里的内容全部复制。

打开：https://github.com/settings/keys

![2021-09-08_103355](D:.\2021-09-08_103355.jpg)

点击 New SSH key

![2021-09-08_103557](D:.\2021-09-08_103557.jpg)

将复制的ssh的key,粘贴到页面按钮key下面的多文本框里，点击添加即可完成。