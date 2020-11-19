# 学习git
## 分支
1. git branch -a 查看所有分支(包括远程)
2. git switch 分支名 :切换分支，该分支必须已经存在，可以是远程分支
3. git checkout -b 分支名: 创建分支并切换到该分支
4. git push origin --delete 分支名 :删除远程分支
## 远程仓库
1. git remote add origin 远程仓库地址: 绑定远程仓库origin
2. git remote -v :查看当前绑定的远程仓库
3. git push -u origin master :第一次将本地分支推送到origin中的master分支，并与之绑定
4. git remote rm origin :删除远程origin仓库 
## 版本回退
1. git restore 文件名 :将工作区恢复为暂存区状态
2. git restore --staged 文件名 :用将暂存区恢复为版本库状态
3. git reset 版本id :回退到版本id,工作区文件不回退，修改未提交到暂存区
4. git reset --hard 版本id :回退到版本id, 工作区文件修改全部撤销
5. git reset --soft 版本id : 回退到版本id， 工作区文件修改提交到暂存区
## 合并
1. git merge 分支名 :将指定分支合并到当前分支
2. git merge --no-ff 分支名 :使用非fast-forward模式合并
3. git rebase

