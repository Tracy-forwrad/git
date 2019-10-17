1.ssh-keygen:创建本地ssh
保存ssh并到GitHub上创建新的密钥: 切换到目录 C:/用户/希望之光/.ssh,复制id_rsa.pub的内容，打开github-》右上角下拉箭头-》settings-》左侧SSH and GPG keys -》new SSH key-》粘贴刚刚的内容
(如果找不到id_rsa.pub文件按，记得查看文件打开"隐藏的文件"选项)
2.本地环境配置
   git config –global user.name ‘xxx’
   git config –global user.email   example@xx.com
   本地name，email设置: C:/用户/希望之光/.gitconfig中可以看到保存的内容
3.git clone  + 远程仓库链接: 克隆远程仓库到本地
4.git remote -v： 查看远程仓库
5.暂存区: 未推送到本地仓库的版本，本地仓库:存在多个版本,工作目录: 呈现出的工作目录
本地分支与远程分支建立关联
git add: 提交希望提交的版本
实例： git add index.html 提交index.html git add .提交到暂存区当前所有的文件 
git commit -m "this a first version": 提交版本并添加描述
6.git status: 查看当前版本状态
7.版本回退
git reset --(soft | mixed | hard)  <HEAD~（num )>  | <commit ID>
soft： 回退到上一个暂存区和本地仓库，与工作目录不一致
mixed： 暂存区和本地工作目录一致，和仓库不一致

8.git reflog: 查看各个版本信息
git remote add origin yougithub
9.一般master分支，是稳定后推送上线的分支，而在其他分支中所作的更改


