#linux命令
pwd 查看所在路径
rm 文件名|夹 删除(只能删除一个文件)
rm -rf 文件名|夹  强制删除
mkdir 文件夹名
ls 展现所有列表
ls -a 显示所有隐藏文件
ls -al 显示文件权限
touch 文件名 创建文件 index.js 都是空文件

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






