#linux命令
pwd 查看所在路径
rm 文件名|夹 删除(只能删除一个文件)
rm -rf 文件名|夹  强制删除
mkdir 文件夹名
ls 展现所有列表
ls -a 显示所有隐藏文件
ls -al 显示文件权限
touch 文件名 创建文件 index.js 都是空文件
cat index.js 控制台打印index.js内容

vi 打开编辑界面
i 切换到 insert 模式
esc 退出 insert模式
:wq 保存退出
:q! 退出不保存

#配置Git 不要早文件夹里嵌套初始化Git
git init -y 初始化Git
git --config --list 显示配置列表
git --config --global user.name xlu
git --config --global user.email luxue008@163.com

#
git status 查看文件状态
git add 文件名
git add . 从工作区添加所有文件到暂存区
git add -A 从工作区添加所有文件到暂存区

git rm --cached  <文件>... 删除暂存区
git rm --cached . -r  递归删除暂存区

git commit -m"message" 从暂存区提交到历史记录区

git commit -a -m"message"  从工作区直接提交到历史记录区

#比较
git diff  工作区和暂存区比较
git diff --cached 暂存区和历史区比较
git diff master 工作区和历史区比较

#撤销
git checkout 文件|名 从暂存区把工作区的修改覆盖
git checkout .

git reset HEAD 文件名 将暂存区的内容向上回滚一次
git reset HEAD .

history > 1.txt 将历史记录写到1.txt中

git log 查看历史记录
git reflog 查看所有的历史，包括移动的，删除的
git log --graph  


git reset --hard db2cf3c7d9604bf5c09a10d9 版本号 从历史区回滚
git reset --hard HEAD^ 将历史记录区向上回滚一次

#分支合并

git branch 查看分支
git branch dev 创建Dev分支
git checkout dev 切换到dev分支
git checkout -b dev 创建Dev分支并且切换到Dev分支上

git branch -D 分支名 删除Dev分支

git stash  当文件有修改时，切换分支是不允许的，此命令可以将修改暂存起来
git stash pop 
git merge dev 主分支合并dev分支


#添加仓库
git remote add origin https://github.com/luxuehai008/gitProject.git //origin 是别名
git push -u origin master // -u origin master 以后就不用写了 直接git push
