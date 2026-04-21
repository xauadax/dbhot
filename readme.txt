#初始化 ，让git帮助我们当前文件夹
git init

#检测当前目录下文件的状态
git status

#三种状态的变化：红—>绿—>生成版本
##红色：新增文件/修改了的老文件—>git add 文件名/ .( .是所有文件都添加进去)
##绿色：git 已经管理起来了—> git commit -m "描述信息"
##生成版本

#查看版本记录
git log

#回滚至之前的版本
git log 
git reset --hard 版本号

#回滚至之后的版本
git reflog 
git reset --hard 版本号

#修改后的文件回到修改前
git checkout

#暂存区（绿色）回到工作区（红色）
git reset HEAD

#查看分支
git branch

#创建分支
git branch 分支命称

#切换分支
git checkout 分支名称

#分支合并（可能产生冲突，找到冲突文件，手动修改）
git merge 要合并的分支 #注意切换分支再合并

#删除分支
git branch -d 分支名称



#工作流



#给远程仓库起名字
git remote add origin 远程仓库地址

#向远程推送代码
git push -u origin 分支

#克隆远程仓库地址
git clone 远程仓库地址（内部已实现git remote add origin 远程仓库地址）

#切换分支
git checkout 分支
