#GIT使用

工作区 ———— 暂存区———— 本地仓库


##readme文档
readme文件可以是TXT文档，也可以是md文档

##全局配置
1.配置用户名
2.配置用户邮箱

1.创建一个文件夹作为工作区
2.打开文件夹 右键 git base here 进入当前目录
3.工作区持有项目实际文件


##初始化
1.get init 初始化版本库
2.当前目录后面有一个括号（master）代表初始化成功
3.在当前目录下会生成一个隐藏文件 .git 代表版本库  （不要修改操作）

##工作区内容提交到本地仓库
1.执行命令 git add 文件名 将工作区的内容提交到暂存区
2.命令 git add . 将所有变动（新增。修改。删除）提交到暂存区
3.从暂存库提交到本地仓库 git commit -m '提交注释'

##版本回退
1.命令 :git reset --hard HEAD^  回退到上一个版本（一个^代表上一个版本）
2.命令：git reset --hard 版本号 回退到指定版本。（回退之前一定要提交当前版本）

##辅助命令
1.命令 git status 查看当前目录下的新
2.git log 查看日志  哈希值，唯一
3.git reflog 查看简版日志——哈希值只有7位


##将本地仓库提交到远程仓库
1.在gitup创建一个远程仓库  git2020
2.本地工作区先提交到本地仓库

3.本地仓库和远程仓库关联
$ git remote add origin https://github.com/SeeUzq/git2020.git
origin 相当于一个变量 
4.git remote -v 查看本地仓库所关联的远程仓库地址
5.git push -u origin master
git push把本地仓库推送到远程仓库
-u origin master 设置默认提交master分支到origin

6.git push -u -f origin master 强制推送到远程 （不推荐，当远程仓库不是空的仓库时（比如添加新仓库时勾了readme），导致本地仓库无法正常推送）


##下载项目到本地
版本库——初始化  ，将本地仓库和远程仓库绑定在一起了


git clone 适用于本地没有，
3.从远程更新达到本地仓库，直接更新命令，git fetch ， 不会自动merge
4.一定要养成工作区的修改提交到到本地仓库，更新远程到本地
jalhfsl




1.每天更新代码
2.可以在线编辑，将导致本地和线上不一致。


12
dev分支代码修改





